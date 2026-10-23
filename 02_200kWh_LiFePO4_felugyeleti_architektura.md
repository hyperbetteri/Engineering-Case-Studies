**Language / Nyelv:** [English](02_200kWh_LiFePO4_felugyeleti_architektura.en.md) · [Magyar](02_200kWh_LiFePO4_felugyeleti_architektura.md)

# 200 kWh-s LiFePO4 energiatároló — adatgyűjtési és felügyeleti architektúra

**Előkészítő műszaki terv**

Szerző: Almási Andor · Alapváltozat: v1.4 (2026. január) · Publikus változat

> **Publikációs megjegyzés.** A publikus változat a rendszer felépítési elveit, az interfész-logikát és a cellaszámítást tartalmazza. A konkrét készletadatok, költség- és munkaidő-kalkulációk, valamint a piaci értékbecslés nem részei a publikus változatnak.

## 1. Projektmegnevezés és alapcél

200 kWh-s LiFePO4 energiatároló rendszer HMI-alapú adatgyűjtési és felügyeleti architektúrája — előkészítő terv.

## 2. Kiindulási keret

| Szempont | Érték |
|---|---|
| Rendszerfeszültség | körülbelül 400 V egyenfeszültség |
| Energiatartalom | 200 kWh |
| Terhelés | legalább 250 A folyamatos |
| Cél | mérési bizonyítékok előállítása, állapotkövetés, dokumentálhatóság, későbbi piacképesség |
| Fázis | adatgyűjtés és tervezés — nem üzembe helyezés |

## 3. Rendszerszintű felosztás és biztonságos szeparáció

**Alapelv:** a védelem, a vezérlés és a megjelenítés **nem azonos szinten** működik.

## 4. Funkcionális rétegek

| Réteg | Elemek |
|---|---|
| 4.1 Cellaszint | cellák, hőérzékelők |
| 4.2 Balanszer és BMS szint | aktív balanszer modulok; cellafeszültség, hőmérséklet, töltöttségi állapot (SOC), hibák |
| 4.3 Adatgyűjtő és vezérlő szint | gateway vagy PLC funkció |
| 4.4 HMI és felügyelet | megjelenítés, naplózás, adatexport |
| 4.5 Külső világ | SCADA, laptop, audit célú hozzáférés |

Ez a felosztás ipari gyakorlat, auditálható és biztosításbarát.

## 5. Interfész-logika

### 5.1. Cellák és balanszer kapcsolata

- Hardver: dedikált aktív balanszer modulok.
- Kapcsolat: a cellák közvetlen feszültség- és hőmérséklet-érzékelő vezetékeken csatlakoznak a balanszer modulokhoz; ezen a szinten nincs kommunikációs protokoll.

A HMI közvetlenül nem avatkozik be ezen a szinten.

### 5.2. Balanszer és adatgyűjtő kapcsolata

- Kommunikáció: RS-485 vonalon Modbus RTU protokollal, vagy CAN buszon (például CANopen vagy a gyártó saját protokollja).
- Indok: determinisztikus működés, zajtűrés, ipari szabvány.
- Feladatok: cellafeszültségek mérése, hőmérsékleti adatok, balanszolási állapot, hibák és események.

**Ez az a réteg, ahol az adat hitelessé válik.**

### 5.3. Gateway és HMI kapcsolata

- Kommunikáció: Ethernet hálózaton.
- Protokoll: Modbus TCP vagy OPC-UA.
- Előnyök: galvanikus leválaszthatóság, skálázhatóság, dokumentálhatóság.

### 5.4. HMI és külső világ kapcsolata

- Adatexport: USB vagy SD adathordozón.
- Hálózati elérés: Etherneten keresztül, SFTP vagy HTTPS protokollal.
- Cél: bizonyíték, mérési jegyzőkönyv, auditanyag.

## 6. A HMI szerepe

**Alapelv:** a HMI nem védelmi eszköz és nem valós idejű balanszer.

A HMI feladatai: adatgyűjtés, naplózás, vizualizáció, műszaki bizonyíték előállítása. Az aktív balanszolás külön hardveren fut; a HMI csak konfigurációt és vezérlést biztosít. Ez a szétválasztás műszakilag és a felelősségi határok szempontjából is tiszta megoldás.

## 7. Az előkészítő felépítés előnyei

- moduláris;
- visszabontható;
- nem zárja le a későbbi döntéseket;
- bővíthető audit vagy CE irányba;
- nem zsákutca.

## 8. Cellaszámítás 120 soros cellára

### 8.1. Egy cella alapadatai

- Névleges feszültség: 3,2 V
- Kapacitás: 100 Ah
- Egy cella energiatartalma: 3,2 V × 100 Ah = **320 Wh**

### 8.2. Soros cellaszám és rendszerfeszültség

- Soros cellák száma: 120
- Névleges rendszerfeszültség: 120 × 3,2 V = **384 V**

### 8.3. Egy soros lánc energiatartalma

- 120 cella × 320 Wh = 38 400 Wh = **38,4 kWh**
- Ellenőrzés: 384 V × 100 Ah = 38,4 kWh — a két módszer azonos eredményt ad.

### 8.4. Közel 200 kWh eléréséhez szükséges párhuzamos ágak

200 kWh / 38,4 kWh ≈ 5,2 → egész ágakkal számolva **5 párhuzamos ág**.

### 8.5. Teljes rendszer 120S5P konfigurációban

- Feszültség: 384 V
- Kapacitás: 5 × 100 Ah = 500 Ah
- Energia: 384 V × 500 Ah = 192 000 Wh = **192 kWh**

### 8.6. Teljes cellaszám

120 soros cella × 5 párhuzamos ág = **600 cella**. Ellenőrzés: 192 000 Wh / 320 Wh = 600 cella.

### 8.7. Következtetés

120 soros cellával a rendszer névleges feszültsége 384 V. Öt párhuzamos ággal a teljes energiatartalom 192 kWh. Ezt a konfigurációt műszakilag helyesen körülbelül 200 kWh-s rendszerként lehet kezelni.

## 9. Szakmai megjegyzés: miért számít a cellaválogatás?

A közel 200 kWh-s, körülbelül 400 V névleges feszültségű energiatároló rendszereknél a folyamatos 250 A-es terhelhetőség nem tekinthető piaci alapértéknek. Tapasztalatunk szerint ilyen paraméterekkel rendelkező akkumulátorpakkok jellemzően csak egyedi megrendelésre érhetők el, és még akkor is ritkák.

A kereskedelmi forgalomban kapható nagy kapacitású rendszerek döntő többsége nem válogatott cellákból vagy csomagokból, hanem gyártási tűréseken belüli, átlagos minőségű egységekből épül fel. A válogatott cellák alkalmazása:

- javítja az árammegoszlást;
- csökkenti a belső feszültségszórást;
- mérhetően növeli a várható élettartamot.

A tervezett rendszereknél konzervatívan **8000 teljes töltési–kisütési ciklussal** lehet számolni. LiFePO4 kémia esetén ez nem optimista, hanem reálisan tartható érték, különösen aktív balanszolással és kontrollált üzemeltetéssel. Egy 192 kWh-s rendszer esetében ez összesen körülbelül **1536 MWh** életciklus alatti energialeadást jelent. A ciklusszám a cellagyártói adatlapon megadott feltételekhez kötött (kisütési mélység, hőmérséklet, áramterhelés, élettartam végi maradó kapacitás); ezektől eltérő üzemben kevesebb is lehet.
