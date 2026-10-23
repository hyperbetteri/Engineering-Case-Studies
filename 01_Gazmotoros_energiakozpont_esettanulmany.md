**Language:** [Magyar](01_Gazmotoros_energiakozpont_esettanulmany.md) | [English](01_Gazmotoros_energiakozpont_esettanulmany.en.md)

# Hőtermelésre optimalizált, gázüzemű belső égésű motoros energiaközpont kísérleti megvalósítása

**Mérnöki esettanulmány**

Szerző: Almási Andor · Kanonikus műszaki változat: 2026. augusztus 5. · Publikus változat

> **Publikációs megjegyzés.** Ez a változat a kanonikus műszaki esettanulmányt tartalmazza. A rendszer fő szellemi értékét képviselő saját konstrukciós megoldás pontos működése, kialakítása és szabályozási elve nem nyilvános (lásd a 7.5. és a 16. fejezetet). A dokumentációs és kapcsolati melléklet nem része a publikus változatnak.

## Vezetői összefoglaló

A jelen esettanulmány egy műhelyalapú, funkcionális újrahasznosítással létrehozott gázüzemű hő- és villamosenergia-termelő prototípust dokumentál.

A rendszer alapját egy elektromos hajtású, gázüzemű Still targoncából kimentett, Volkswagen Polo eredetű, 1,6 literes, négyhengeres Ottó-motor és a hozzá tartozó 48 voltos villamos generátor képezte.

A donor targonca belső vezetékhálózata egy korábbi elektromos kábel- és vezetéktűz következtében súlyosan károsodott. A járművet már nem állították helyre, de a belső égésű motor, a generátor és több kapcsolódó gépészeti részegység sértetlen és működőképes maradt. Ezek a részegységek bontás vagy beolvasztás helyett egy új energetikai rendszerben kaptak második funkcionális életciklust.

A fejlesztés célja nem az Ottó-motor mechanikai teljesítményének maximalizálása volt. Ennek ellenkezője történt: a motort szándékosan olyan extrém alacsony fordulatszámú üzemállapotban működtettük, amelyben a tüzelőanyag energiájának túlnyomó része hőként jelent meg.

A koncepció röviden:

- az eredendően mérsékelt mechanikai hatásfokú Ottó-motort nem próbáltuk nagy teljesítményű erőgéppé fejleszteni;
- a mechanikai energia arányát tudatosan alacsonyan tartottuk;
- a motorblokkban, a hűtőfolyadékban és a kipufogógázban keletkező hőt visszanyertük;
- a berendezést elsődlegesen dugattyús gázkazánként használtuk;
- a villamos energia másodlagos, de hasznos melléktermék volt.

A rendszer hitelesített gázórával mérve megközelítőleg 3 m³ földgázt fogyasztott óránként. A stabil üzemi fordulatszámot folyamatosan lézeres fordulatszámmérővel ellenőriztük. Az optimális tartomány 350–450 fordulat/perc volt, jellemzően 400–410 fordulat/perces működéssel.

A prototípus két teljes téli fűtési szezonban működött. Az egyes üzemmenetek néhány órától több tíz óráig tartottak. A rendszer hozzávetőleg 450 m² összesített területű műhely-, raktár- és közösségi épületegyüttest fűtött, egy folyamatosan bekötött, körülbelül 1 m³ térfogatú puffertartályon és kiterjedt radiátoros csőhálózaton keresztül.

A korabeli teljesítménymérések nem érték el egy mai laboratóriumi vizsgálat műszerezettségi szintjét. Emiatt a dokumentum világosan elkülöníti:

- a közvetlenül mért adatokat;
- a hosszabb üzemben megfigyelt jelenségeket;
- az utólag kiszámítható értékeket;
- a becsült paramétereket;
- valamint a nem nyilvános konstrukciós megoldásokat.

A rendelkezésre álló adatok alapján a prototípus működése termodinamikailag és gépészetileg konzisztens. A pontos összesített hatásfok utólag nem állapítható meg, de a nagy hőteljesítmény, a stabil tartós működés és a motor hűtőköri, valamint kipufogóoldali hőjének együttes hasznosítása mérnökileg igazolható.

## 2. A fejlesztés szemléleti alapja

### 2.1. Funkcionális újrahasznosítás

A fejlesztés egyik elsődleges alapelve az volt, hogy a rendszer ne előre meghatározott, újonnan beszerzendő alkatrészekből épüljön fel. A tervezési folyamat abból indult ki, hogy:

- milyen működőképes részegységek találhatók a környezetben;
- ezek milyen eredeti funkcióra készültek;
- milyen más funkcióban használhatók fel;
- milyen minimális átalakítás szükséges az új rendszerbe történő integrációhoz.

A szemléletet egy családi példázat foglalja össze:

> „Nem kell megvenni egy egész tehenet ahhoz, hogy az ember megigyon egy pohár tejet.”

Ennek műszaki jelentése nem az alkalmi vagy igénytelen kivitelezés volt, hanem az, hogy először a rendelkezésre álló erőforrásokban rejlő funkcionális lehetőségeket kell felismerni. Csak azt kell újonnan beszerezni vagy legyártani, ami valóban nem helyettesíthető meglévő eszközzel.

A donor targoncából származó motor és generátor ennek az értékmentő logikának megfelelően került felhasználásra. Mindkét főegység hibátlan működési állapotban volt, noha az eredeti járművet a vezetéktűz miatt már bontásra szánták.

### 2.2. Műhelyalapú fejlesztés

A prototípus nem formális kutatás-fejlesztési programban, nem laboratóriumban és nem teljes körű előzetes mérnöki dokumentáció alapján készült.

A fejlesztők rendelkeztek:

- gépészeti és villamos gyakorlati ismeretekkel;
- szerelési és műhelytapasztalattal;
- működőképes műszaki intuícióval;
- különféle ipari alkatrészekhez és szerszámokhoz való hozzáféréssel.

Nem állt azonban rendelkezésre:

- teljes kalorimetrikus mérőrendszer;
- hitelesített nyomatékmérő fékpad;
- folyamatos füstgázelemzés;
- minden hőköri ponton telepített hőmérséklet- és térfogatáram-mérés;
- előzetesen elkészített numerikus áramlástani modell.

A konstrukció iteratív módon alakult ki: rendelkezésre álló alkatrészek kiválasztása → mechanikai összeillesztés → próbaüzem → megfigyelés → szabályozás és módosítás → ismételt hosszabb üzemi vizsgálat.

Ez a módszer nem azonos a szabványos ipari termékfejlesztéssel, de alkalmas volt annak bizonyítására, hogy az alapelv a valóságban működő rendszerként megvalósítható.

## 3. A donorberendezés és a fő részegységek

### 3.1. A donor Still targonca

A donorberendezés egy villamos hajtású, gázüzemű Still targonca volt. A targonca működési elve szerint a belső égésű motor egy 48 voltos generátort hajtott, amely a jármű villamos rendszerének energiaellátását biztosította.

A targonca belső vezetékezése korábban leégett. A károsodás nem érintette érdemben:

- a Volkswagen-eredetű belső égésű motort;
- a 48 voltos generátort;
- a fő mechanikai egységeket;
- több kapcsolódó szabályozó- és hajtáselemet.

A donorberendezés pontos gyártási éve nem ismert. A motor a kísérlet idején már régebbi konstrukció volt, de mechanikailag használható állapotban maradt.

### 3.2. Belső égésű motor

A hajtógép fő adatai:

| Jellemző | Adat |
|---|---|
| Eredet | Volkswagen Polo konstrukció |
| Hengerűrtartalom | körülbelül 1,6 liter |
| Hengerszám | négy |
| Működési elv | négyütemű Ottó-motor |
| Eredeti üzemanyag | benzin vagy gázüzemre alkalmas kialakítás |
| Kísérleti üzemanyag | először PB-gáz, később hálózati földgáz |
| Keverékképzés | karburátoros rendszer |
| Gázbevezetés | a karburátor levegőoldalán |
| Gyújtás | megszakítóalapú, részben mechanikus, részben elektronikus rendszer, feltehetően Hall-jeladós vezérléssel |

A gyújtórendszer pontos típusa utólag nem azonosítható teljes bizonyossággal. A biztosan rekonstruálható lényeg az, hogy a szikraképzés nem kizárólag hagyományos mechanikus elosztással történt, hanem elektronikus kapcsolási fokozat is részt vett benne.

### 3.3. Generátor és villamos kapcsolat

A motorhoz eredetileg tartozó 48 voltos generátort megtartottuk. A generátor:

- közvetlen mechanikai kapcsolatban állt a motorral;
- áttétel nélkül működött;
- a motortengellyel azonos nagyságrendű fordulatszámon forgott;
- lüktető egyenfeszültségű kimenetet szolgáltatott;
- ólomsavas akkumulátorcsoport töltésére csatlakozott;
- időszakosan körülbelül 1 kW nagyságrendű villamos fogyasztót is ellátott.

A villamos kimenethez Graetz-híd, egyenirányító diódák és több tízezer mikrofarad kapacitású DC-köri pufferkondenzátor kapcsolódott. A pufferkondenzátor feladata:

- a generátor lüktető kimenetének simítása;
- a DC–DC átalakító stabilabb bemeneti táplálása;
- a pillanatnyi feszültségingadozások mérséklése;
- a kapcsolt terhelések tranziens igényének részbeni fedezése.

A rendszer kezdetben nehezebben indult, amíg a nagy kapacitású kondenzátor fel nem töltődött. Ez megfelel annak, hogy a kondenzátor üres állapotban rövid ideig nagy bekapcsolási áramot igényelt.

### 3.4. Lendítőkerék és tengelykapcsolat

A motor főtengelye és a generátor között körülbelül 80 kg tömegű, külön csapágyazott lendítőkerék helyezkedett el. A mechanikai kapcsolat elemei:

- csapágyazott lendítőkerék;
- Hardy-tárcsa vagy hasonló rugalmas tengelykapcsoló elem;
- körmös tengelykapcsoló;
- minimális esztergályos illesztés;
- közvetlen hajtás, áttétel nélkül.

A lendítőkerék szerepe alapvető volt. Az extrém alacsony fordulatszám miatt az egyes hengerek munkaütemei között jelentős szögsebesség-ingadozás alakulhatott volna ki. A nagy tehetetlenségi nyomatékú lendítőkerék:

- energiát tárolt a munkaütem alatt;
- visszaadta az energiát a kompressziós és kipufogási ütemek során;
- egyenletesebbé tette a főtengely forgását;
- csökkentette a lefulladás veszélyét;
- mérsékelte a hajtáslánc impulzusszerű terhelését;
- stabilizálta a generátor feszültségét;
- csökkentette a rezgéseket és a zajt.

A lendítőkerék pontos átmérője és tömegeloszlása nem dokumentált. Emiatt a tárolt forgási energia nem számítható ki megbízhatóan, de a körülbelül 80 kg-os tömeg alapján a stabilizáló hatás jelentős lehetett.

## 4. A koncepció termodinamikai logikája

### 4.1. Nem a mechanikai hatásfok maximalizálása volt a cél

Egy hagyományos belső égésű motor fejlesztésekor általában az a cél, hogy a tüzelőanyag energiájának minél nagyobb része jelenjen meg hasznos tengelyteljesítményként. Ebben a projektben eltérő célfüggvényt alkalmaztunk. A cél az volt, hogy:

- a motor csak annyi mechanikai teljesítményt termeljen, amennyi saját működéséhez, a generátor hajtásához és a stabil terheléshez szükséges;
- a tüzelőanyag energiájának nagyobb része a motorblokkban és a kipufogógázban jelenjen meg hőként;
- ezt a hőt a lehető legnagyobb arányban a fűtési rendszerbe vezessük.

A mechanikai hatásfok tudatos csökkentése tehát nem az összesített energiahasznosítás csökkentését jelentette. A rendszer célja az energiakimenet megoszlásának átalakítása volt: kisebb villamos és mechanikai rész, nagyobb visszanyerhető hőrész.

### 4.2. Belső égésű, dugattyús gázkazán

A rendszer funkcionálisan egy olyan gázkazánként értelmezhető, amelyben az égés nem folyamatos égőtérben, hanem hengerekben, periodikus kompresszióval és gyújtással történt. A motor ebben az üzemállapotban egyszerre biztosította:

- a gáz-levegő keverék beszívását;
- a keverék sűrítését;
- az égés vezérelt időzítését;
- a hő átadását a motorblokk és a hűtőfolyadék felé;
- a forró égéstermék továbbítását a kipufogó-hőcserélő felé;
- korlátozott mechanikai és villamos melléktermelést.

### 4.3. Kapcsolt energiatermelési besorolás

A rendszer műszakilag kapcsolt hő- és villamosenergia-termelő (CHP) prototípusnak tekinthető. A teljes CHP-hatásfok általános definíciója:

```
η_össz = (P_el + Q_hasznos hő) / P_üzemanyag
```

ahol P_el a nettó hasznos villamos teljesítmény, Q_hasznos hő a ténylegesen hasznosított hőteljesítmény, P_üzemanyag a tüzelőanyag által bevitt teljesítmény.

A CHP-rendszerekben a motor kipufogógázából, hűtőközegéből és esetenként kenőolajából is visszanyerhető hő. Ez nem egyedi vagy fizikailag rendellenes eljárás, hanem a dugattyús motoros kapcsolt energiatermelés ismert alapelve. Az EPA műszaki katalógusa szerint a dugattyús motor hője több forrásból, így a kipufogóból és a köpenyvízből is visszanyerhető.

A korabeli prototípus sajátossága az volt, hogy ezt az elvet szokatlanul alacsony fordulatszámon és kifejezetten hőtermelésre optimalizált üzemállapotban alkalmazta.

## 5. Üzemanyag-ellátás

### 5.1. PB-gázos kezdeti próbák

A rendszer első próbái PB-gázzal történtek. A korábbi összegzésben 2 m³/h PB-gázfogyasztás szerepelt. Ez az adat a jelen visszaemlékezés alapján nem kezelhető ugyanolyan bizonyosságú mért adatként, mint a földgázfogyasztás. Ezért a PB-gázos fogyasztási érték csak korabeli becslésként vagy előzetes próbaadatként használható.

### 5.2. Földgázüzem

A későbbi, tartós üzem hálózati földgázzal történt. A gázfogyasztást külön beépített, hitelesített gázórával mértük.

Mért földgázfogyasztás: **V̇gáz ≈ 3 m³/h**

34 MJ/m³ alsó fűtőértékkel számolva:

```
P_be = 3 m³/h × 34 MJ/m³ = 102 MJ/h
1 kWh = 3,6 MJ  →  P_be = 102 / 3,6 ≈ 28,33 kW
```

A 3 m³/h fogyasztás tehát hozzávetőleg 28,3 kW tüzelőanyag-oldali teljesítményt jelentett. A tényleges földgáz fűtőértéke hálózati összetételtől és elszámolási állapottól függően változhat. Emiatt mérnöki becslésként célszerű körülbelül 27–30 kW bemenő teljesítménnyel számolni.

## 6. Fordulatszám és üzemállapot

### 6.1. Mért üzemi fordulatszám

A motor fordulatszámát lézeres fordulatszámmérővel folyamatosan ellenőriztük.

- Mért jellemző üzemi érték: **400–410 fordulat/perc**
- Tapasztalatilag használható tartomány: **350–450 fordulat/perc**

A fordulatszámot mechanikus szabályozással tartottuk stabilan.

### 6.2. Az 500 fordulat/perc fölötti tartomány

Amikor a motor fordulatszámát 500 fordulat/perc fölé emeltük:

- az öntvény kipufogócsonk vörös izzásba került;
- a hőcserélőhöz kapcsolódó cső rendkívüli hőterhelést kapott;
- a csatlakozás részben megolvadt vagy leszakadt;
- a csövet később vissza kellett hegeszteni.

Ez az állapot nem üzemszerű tartomány volt. A vörös izzás pontos hőmérséklete nem ismert. A megfigyelés azonban egyértelműen jelzi, hogy a kipufogóoldali hőterhelés 500 fordulat/perc felett gyorsan és elfogadhatatlan mértékben emelkedett.

A 400–410 fordulat/perc körüli beállítás ezért nem önkényes választás volt, hanem tapasztalati optimalizálás eredménye: stabil égés, kezelhető termikus terhelés, megfelelő generátorterhelés, alacsony zaj, egyenletes működés, hosszabb távú üzembiztonság.

## 7. Hővisszanyerő rendszer

### 7.1. Hőforrások

A rendszer két fő hőforrást hasznosított: a motorhűtési hőt és a kipufogógáz hőtartalmát. A dugattyús motoros CHP-rendszerekben a köpenyvíz és a kipufogógáz együttes hőhasznosítása műszakilag ismert megoldás. A motor kipufogógáza magasabb hőmérsékletű, míg a hűtőkör stabilabb, alacsonyabb hőmérsékletszintű hőforrást biztosít.

### 7.2. Lemezes hőcserélő

A prototípusban egy új állapotú, hozzávetőleg 400 kW névleges kapacitású, valószínűleg Alfa Laval gyártmányú professzionális lemezes hőcserélőt használtunk. A 400 kW-os névleges érték nem a motor tényleges hőteljesítményét jelenti.

A hőcserélő kiválasztásának fő oka az volt, hogy:

- a rendelkezésre álló kisebb egység csatlakozásai elégtelenek voltak;
- a nagy egység több mint 1 colos be- és kimeneti csatlakozásokkal rendelkezett;
- a füstgáz átvezetéséhez megfelelő keresztmetszet kellett;
- kerülni kellett a túlzott kipufogóoldali ellennyomást;
- a kisebb áramlási keresztmetszet lefékezhette volna a füstgáz távozását;
- a fojtás ronthatta volna az égést és a motor stabilitását.

Gázoldali hőcserélőknél az alacsony nyomásveszteség valóban meghatározó tervezési szempont. A hőcserélő tényleges kiválasztását tehát nem a 400 kW-os hőigény, hanem az elérhető portméret, áramlási keresztmetszet és kis gázoldali ellenállás határozta meg.

### 7.3. Közegszétválasztás

A füstgáz nem keveredett a fűtővízzel vagy a motor hűtőfolyadékával. A hőcserélő elkülönített járatrendszereiben az egyik oldalon a forró füstgáz, a másik oldalon a folyadékkör haladt. A pontos belső lemezkiosztás és járatrendszer utólag nem rekonstruálható. A bekötésnél azonban tudatosan ügyeltünk arra, hogy az oldalak ne legyenek keresztbekötve, és a közegek ne keveredjenek.

### 7.4. Motorhűtési kör

A motor saját folyadékhűtő rendszerét szintén a hőhasznosító rendszerhez kapcsoltuk. A motorhűtés feladata kettős volt: a motor üzemi hőmérsékletének stabil tartása és a motorblokkban keletkező hő fűtési célú hasznosítása.

A több hónapos, ismétlődő téli üzem alapján a hőelvonás tartósan megfelelő volt. Nem csak rövid demonstráció történt: a motor néhány órás és több tíz órás megszakítás nélküli üzemmenetekben is működött.

### 7.5. Nem nyilvános konstrukciós megoldás

A rendszer magas hőhasznosítását nem kizárólag a nagy hőcserélő alkalmazása eredményezte. A teljes konstrukció tartalmazott olyan saját műszaki megoldást vagy megoldáscsoportot, amely:

- meghatározta a motor tényleges termikus üzemállapotát;
- befolyásolta az égés, a fordulatszám és a hőelvonás kapcsolatát;
- lehetővé tette a hűtőköri és kipufogóoldali energia kedvező hasznosítását;
- a rendszer fő szellemi és műszaki értékét képviseli.

Ennek pontos működési módja, geometriai kialakítása, kapcsolása és szabályozási elve nem nyilvános. A tanulmány ezért csak a rendszer külső energiamérlegét és dokumentálható működését ismerteti. A kulcsfontosságú saját megoldás nem kerül részletezésre, és helyét nem szabad feltételezett vagy utólag kitalált magyarázattal kitölteni.

## 8. Fűtési rendszer

### 8.1. Fűtött komplexum

A rendszer Debrecenben egy nagyméretű épületegyüttest fűtött. A komplexum három fő részből állt: műhely, nagyméretű raktár, valamint konyha–étkező–közösségi tér.

A teljes fűtött alapterület megközelítőleg **450 m²**. A pontos érték néhány négyzetméterrel eltérhetett, de a 450 m²-es nagyságrend reális.

### 8.2. Konyha–étkező–közösségi tér

A legjobban dokumentálható külön helyiség:

- alapterület: legalább 80 m²;
- belmagasság: körülbelül 2,4 m;
- becsült légtérfogat: legalább 192 m³ (80 m² × 2,4 m);
- eredeti funkció: garázs;
- későbbi funkció: hőszigetelt konyha, étkező és családi közösségi tér.

A helyiségben rendszeresen több ember tartózkodott. Egy próba során a hőmérséklet olyan magasra emelkedett, hogy a jelenlévők kérték a rendszer leállítását.

### 8.3. Csőhálózat

A fűtési hálózat kiterjedt, több épületrészt kiszolgáló rendszer volt. A pontos csőhossz nem dokumentált. A visszaemlékezés alapján legalább 100 méteres nagyságrend biztosan fennállt, és a teljes hossz ennél lényegesen nagyobb is lehetett. A korábban említett 450 méteres becslés nem igazolható, de a nagy komplexum miatt nem zárható ki.

A helyes meghatározás: *„legalább százméteres, valószínűleg több száz méteres összesített csőhálózat”*.

### 8.4. Puffertartály

A rendszerhez körülbelül 1 m³, azaz 1000 liter térfogatú puffertartály kapcsolódott. A puffertartály:

- folyamatosan a fő vízkörben volt;
- nem volt üzemszerűen kikerülve;
- jelentős termikus tehetetlenséget biztosított;
- csökkentette a hirtelen hőmérséklet-ingadozásokat;
- lehetővé tette a motor folyamatos működését változó hőigény mellett.

### 8.5. Keringetés

Két keringetőszivattyút alkalmaztunk: a motor–hőcserélő kör szivattyúját és az épület radiátoros körének szivattyúját. A szivattyúk fordulatszámát és az áramlási viszonyokat kísérleti úton szabályoztuk. A cél az volt, hogy:

- a motor hőmérséklete stabil maradjon;
- a hőcserélő megfelelő hőlépcsővel működjön;
- a radiátoros körben elegendő tömegáram legyen;
- ne alakuljon ki túl gyors lokális forrás vagy elégtelen hőelvonás;
- a puffertartály és az épületi kör között megfelelő energiaszállítás történjen.

### 8.6. Nyomásviszonyok

A fűtési rendszer zárt rendszerként működött. Jellemző nyomás: tartósan 2 bar fölött, magas hőterhelésnél megközelítőleg 3 bar. A nyomás pontos időfüggése és a biztonsági szerelvények teljes konfigurációja utólag nem dokumentálható.

A közel 3 bar nyomás azt mutatja, hogy a rendszer a nagy hőterhelés során a hagyományos zárt fűtési rendszerek felső üzemi tartományához közelített.

## 9. Hőenergia-számítások

### 9.1. Egyórás tüzelőanyag-energia

```
E_1h = 3 m³ × 34 MJ/m³ = 102 MJ  ≈ 28,33 kWh
```

Egy óra alatt tehát hozzávetőleg 28,3 kWh tüzelőanyag-energia került a rendszerbe.

### 9.2. Az 1000 literes puffer elméleti felmelegítése

A víz fajhője c_p ≈ 4,184 kJ/(kg·K), a puffertartály víztömege m ≈ 1000 kg, az induló vízhőmérséklet a visszaemlékezés szerint T₀ ≈ 16–18 °C (a számításban 17 °C).

Ha az összes bevitt energia kizárólag az 1000 liter vizet melegítené, veszteség és más hőtároló tömeg nélkül, akkor egy óra alatt:

```
ΔT = 102 000 kJ / (1000 kg × 4,184 kJ/kgK) ≈ 24,4 °C
T₁ ≈ 17 + 24,4 ≈ 41,4 °C
```

Ez csak idealizált számítás. A valóságban az energia egyidejűleg került a puffertartályba, a radiátorokba, a csövekbe, a helyiségek levegőjébe, az épületszerkezetbe, a motor és a hőcserélő fémanyagába, valamint részben a környezetbe.

### 9.3. Elméleti felfűtési idők

1000 liter víz 17 °C-ról történő, veszteségmentes felmelegítésének elméleti ideje 28,33 kW teljesítménnyel:

| Célhőmérséklet | ΔT | Szükséges energia | Elméleti idő |
|---|---|---|---|
| 40 °C | 23 K | ≈ 26,73 kWh | ≈ 0,94 óra |
| 50 °C | 33 K | ≈ 38,35 kWh | ≈ 1,35 óra |
| 60 °C | 43 K | ≈ 49,98 kWh | ≈ 1,76 óra |
| 70 °C | 53 K | ≈ 61,60 kWh | ≈ 2,17 óra |
| 80 °C | 63 K | ≈ 73,22 kWh | ≈ 2,58 óra |

Ezek a számok nem jelentik azt, hogy a radiátorok csak a puffer teljes átlaghőmérsékletének elérése után melegedhettek fel. Az előremenő ág hőmérséklete magasabb lehetett a puffer átlagánál, nem történt feltétlenül azonnali tökéletes keveredés, a radiátorok belépő részei közvetlenül magas hőmérsékletű vizet kaphattak, és a helyi felületi hőmérséklet jelentősen meghaladhatta a teljes víztér átlaghőmérsékletét.

Ezért az a megfigyelés, hogy valamivel több mint egy órán belül egyes radiátorok rendkívül forróvá váltak, nem mond ellent az energiamérlegnek.

### 9.4. A 450 m²-es komplexum fűtési terhelése

A teljes épület pontos hővesztesége nem rekonstruálható, mert nem ismert minden épületrész falazata, szigetelési szintje, nyílászárói, a külső hőmérséklet, a légcsere és a belső hőterhelés.

A 28–30 kW-os tüzelőanyag-bemenet 450 m²-re vetítve: 28 300 W / 450 m² ≈ **62,9 W/m²**.

Ez a fajlagos bemenő teljesítmény alkalmas lehetett mérsékelten szigetelt nagy épületegyüttes temperálására, műhely és raktár fűtésére, jól szigetelt közösségi helyiség gyors túlmelegítésére — különösen akkor, ha nem minden tér azonos belső hőmérsékletre volt fűtve.

A 80 m²-es konyha–étkezőre vetítve a teljes 28,3 kW természetesen nem alkalmazható, mert a rendszer egyszerre több teret fűtött. Az azonban valószínű, hogy az adott helyiségben nagy radiátorteljesítmény és magas előremenő hőmérséklet állt rendelkezésre.

## 9/A. A teljes rendszer termikus tehetetlensége és a ciklikus hőtartás

### 9/A.1. A kiegészítés célja

A prototípus működésének helyes értékeléséhez külön kell választani: a hideg vagy részben lehűlt rendszer kezdeti felfűtését; a teljes vízkör, a radiátorok és az épületszerkezet átmelegedését; az ezt követő hőtartási üzemet; és a motor rövid idejű, ciklikus utánfűtéseit.

A korábbi energiaszámítások önmagukban csak azt mutatták meg, hogy adott mennyiségű földgáz elégetésével elméletileg mennyi energia vihető be a rendszerbe. Nem mutatták meg megfelelően, hogy a prototípus nem folyamatos, állandó teljesítményű kazánként működött. A valós üzemben a motor hosszabb kezdeti felfűtést követően csak időszakosan indult el. A hőellátás jelentős részét a motor leállított állapotában a korábban felmelegített, nagy termikus tömegű rendszer biztosította.

Ez a kiegészítés nem változtatja meg az energiamegmaradás törvényét, és nem állítja, hogy a hőtároló tömeg önmagában energiát termelt. Azt magyarázza meg, hogyan tette lehetővé a nagy hőtároló kapacitás:

- a motor kedvező, stabil munkapontban történő üzemeltetését;
- a folyamatos részterhelés elkerülését;
- a ritkább és rövidebb utánfűtési ciklusokat;
- a teljes épületegyüttes lassú lehűlését;
- a pillanatnyi 3 m³/h gázfogyasztásnál jóval kisebb időátlagos fogyasztást.

### 9/A.2. A termikus tömeg fő összetevői

A rendszer hőtároló képességét nem kizárólag az 1 m³-es puffertartály adta. A teljes termikus tömeghez hozzájárult: körülbelül 1000 liter víz a puffertartályban; a legalább százméteres, valószínűleg több száz méteres csőhálózat víztartalma; a radiátorokban található víz; a puffertartály, a csövek és a radiátorok fémanyaga; a motorblokk és a hőcserélő tömege; a műhely, a raktár és a közösségi helyiség padlója, falazata és berendezései; valamint a megközelítőleg 450 m²-es épületegyüttes teljes átmelegített szerkezeti tömege.

A pontos teljes víztérfogat és szerkezeti hőkapacitás nem dokumentált, ezért az összesített hőtárolás nem számítható ki egyetlen pontos értékkel. Az 1000 literes puffer azonban önmagában is alkalmas a rendszer termikus tehetetlenségének alsó becslésére.

### 9/A.3. Az 1000 literes puffertartály hőtárolása

```
Q = m × c_p × ΔT
Q_1K = 1000 × 4,184 / 3600 ≈ 1,162 kWh  (minden 1 °C változásra)
```

| Hőmérséklet-különbség | Tárolt hő |
|---|---|
| 5 °C | ≈ 5,81 kWh |
| 10 °C | ≈ 11,62 kWh |
| 20 °C | ≈ 23,24 kWh |
| 30 °C | ≈ 34,86 kWh |
| 40 °C | ≈ 46,48 kWh |

Például ha a puffer átlaghőmérséklete 80 °C-ról 60 °C-ra csökkent, akkor csak a puffer víztömege körülbelül 83 680 kJ ≈ 23,24 kWh hőt adott le. Ehhez hozzáadódott a csőhálózatban, radiátorokban, fémalkatrészekben és az épületszerkezetben eltárolt energia.

### 9/A.4. A teljes vízkör becsült többletkapacitása

A pufferen kívüli vízmennyiség pontos értéke nem ismert. Szemléltető becslésként 20 °C-os hőlépcsőn: további 100 liter víz ≈ 2,32 kWh, 200 liter ≈ 4,65 kWh, 300 liter ≈ 6,97 kWh, 500 liter ≈ 11,62 kWh energiát tárol.

Amennyiben a puffertartályon kívüli cső- és radiátorkör például 200–400 liter vizet tartalmazott, akkor 20 °C használható hőmérséklet-tartományban a teljes vízkör hőtárolása megközelítőleg 1200 liter esetén 27,89 kWh, 1300 liter esetén 30,21 kWh, 1400 liter esetén 32,53 kWh. Ez csak szemléltető tartomány; a tényleges víztérfogat hiányában nem kezelhető mért adatként.

### 9/A.5. Az épületszerkezet hőtároló hatása

A fűtött épület nem kizárólag a levegőből álló hőterhelést jelentett. A felfűtési szakaszban energiát vett fel a falazat, a betonpadló, a födém, a gépek és raktári tárgyak, a bútorzat, valamint a radiátorok és csővezetékek fémanyaga. A helyiség levegőjének hőkapacitása ezekhez képest viszonylag kicsi.

A közösségi tér kb. 192 m³ levegője (≈ 230 kg, c ≈ 1,0 kJ/(kg·K)) 10 °C-kal történő felmelegítéséhez mindössze kb. 2300 kJ ≈ 0,64 kWh szükséges. Maga a levegő tehát gyorsan felmelegíthető. A rendszer lassú lehűlését nem a levegő, hanem elsősorban a víztömeg, a radiátorok, a csővezetékek, az épületszerkezetek és a teljes komplexum nagy fizikai tömege okozta.

### 9/A.6. A felfűtési és a hőtartási energia különbsége

A hidegindításos felfűtés során nemcsak az épület pillanatnyi hőveszteségét kellett pótolni, hanem energiát kellett bevinni a hideg vízkörbe, a puffertartályba, a radiátorokba, a csövekbe, a motor és a hőcserélő anyagába és az épület lehűlt szerkezeteibe is.

A hőtartási szakaszban azonban a rendszer már fel volt töltve termikus energiával. Ekkor a motor fő feladata már csak az épület pillanatnyi hőveszteségének pótlása, a puffer lassú hőmérséklet-csökkenésének kompenzálása és a radiátoros kör kívánt előremenő hőmérsékletének helyreállítása volt. Ezért a felfűtéshez szükséges teljesítmény és üzemidő nem hasonlítható közvetlenül a későbbi hőtartási fogyasztáshoz.

### 9/A.7. A motor ciklikus üzeme

A motor fordulatszáma 350 fordulat/perc alá nem volt üzembiztosan csökkenthető, mert az égés egyenetlenebbé válhatott, csökkent a lendítőkerék stabilizáló hatása, nőtt a lefulladás kockázata, a generátor és a mechanikai hajtás terhelése arányaiban nagyobbá vált, és romolhatott a kenés és a gázcsere egyenletessége.

A rendszer ezért nem tudta a hőteljesítményt egy korszerű modulációs kazánhoz hasonlóan fokozatmentesen, nagyon alacsony szintre csökkenteni. A szabályozás gyakorlati módja a ciklikus üzem lett:

1. a motor beindítása;
2. működés 400–410 fordulat/perces stabil tartományban;
3. a puffer és az előremenő víz utánfűtése;
4. a motor leállítása;
5. hőleadás a pufferből és a teljes rendszerből;
6. újraindítás a hőmérséklet csökkenésekor.

A motor tehát rövid ideig magas, stabil teljesítményen működött, majd hosszabb ideig állt.

### 9/A.8. Az időátlagos gázfogyasztás

A motor működés közbeni mért földgázfogyasztása körülbelül 3 m³/h. A hőtartási időszak átlagos fogyasztását azonban az óránkénti tényleges működési idő határozta meg:

```
V̇_átlag = V̇_üzem × t_ü     (t_ü = az egy órán belüli üzemidő aránya)
```

| Óránkénti üzemidő | t_ü | Átlagos gázfogyasztás | Átlagos tüzelőanyag-teljesítmény |
|---|---|---|---|
| 5 perc | 0,083 | ≈ 0,25 m³/h | ≈ 2,36 kW |
| 10 perc | 0,167 | ≈ 0,50 m³/h | ≈ 4,72 kW |
| 15 perc | 0,25 | ≈ 0,75 m³/h | ≈ 7,08 kW |
| 20 perc | 0,333 | ≈ 1,00 m³/h | ≈ 9,44 kW |
| 30 perc | 0,50 | ≈ 1,50 m³/h | ≈ 14,17 kW |

A visszaemlékezés szerint előfordult, hogy a motort óránként csak néhány percre vagy körülbelül tíz percre kellett beindítani. Ennek alapján a már átmelegedett rendszer hőtartási szakaszában az órára vetített átlagos gázfogyasztás egyes időszakokban megközelítőleg 0,25–0,50 m³/h tartományba kerülhetett; ez 24 órára vetítve 6–12 m³/nap.

Ezek kizárólag a megadott ciklusidőkből számított példák. Nem tekinthetők teljes téli szezonra vonatkozó dokumentált fogyasztási adatoknak, mert az üzemidő függött a külső hőmérséklettől, a fűtött területek pillanatnyi használatától, a radiátorszelepek állapotától, a szivattyúk beállításától és a puffer kapcsolási hőmérsékleteitől.

Ez magyarázza, hogyan lehetett a motor pillanatnyi, körülbelül 28 kW-os bemenő teljesítménye mellett a teljes épületegyüttes hosszabb távú átlagos hőigénye lényegesen kisebb. A motor rövid idejű működése alatt nagy hőteljesítménnyel töltötte a termikus tárolót, majd a tárolt energia hosszabb idő alatt került az épületbe.

### 9/A.9. A hőtárolásból fedezhető üzemszünet

Csak az 1000 literes puffert vizsgálva, 20 °C használható hőmérséklet-különbséggel (Q ≈ 23,24 kWh) az elméleti hőellátási idő:

| Átlagos hőigény | Elméleti idő |
|---|---|
| 4 kW | ≈ 5,81 óra |
| 6 kW | ≈ 3,87 óra |
| 8 kW | ≈ 2,91 óra |
| 10 kW | ≈ 2,32 óra |
| 15 kW | ≈ 1,55 óra |

A tényleges rendszerben a radiátorok, csövek és épületszerkezetek további energiát tároltak, ezért a helyiségek érzékelhető lehűlése ennél hosszabb idő alatt következhetett be. A számítás azt is igazolja, hogy az óránként néhány perces utánfűtés fizikailag lehetséges lehetett, amennyiben az épület pillanatnyi hővesztesége alacsonyabb volt, a puffer nagyobb hőmérséklet-tartományban működött, a szerkezeti tömeg már átmelegedett, és az időjárás nem jelentett maximális téli terhelést.

### 9/A.10. Miért nem tudott gyorsan lehűlni a rendszer?

A folyamatosan működő keringetőszivattyúk nem akadályozták meg a rendszer teljes energiavesztését, de egyenletesebben elosztották az eltárolt hőt: csökkent a puffer és a radiátorkör közötti hőmérséklet-különbség, a forró víz továbbra is eljutott a távoli radiátorokhoz, a teljes víztömeg együtt vett részt a hőleadásban, és csökkent a helyi gyors kihűlés.

A szivattyú nem termelt hőt, és a keringetés önmagában nem javította a termodinamikai hatásfokot. A rendelkezésre álló hőenergiát azonban jobban elosztotta, és késleltette, hogy egyes távoli vagy kis víztérfogatú szakaszok gyorsan kihűljenek.

### 9/A.11. A magas előremenő hőmérséklet szerepe

A rendszer egyik megfigyelt sajátossága az extrém magas radiátor- és előremenő hőmérséklet volt. Ennek következtében a radiátorok fajlagos hőleadása jelentősen megnőtt, a helyiségek gyorsan felmelegedtek, és a 400–410 fordulat/perces motorüzem túl nagy hőteljesítményt jelentett az adott pillanatnyi hőigényhez képest — a rendszer ezért ciklikus szabályozást igényelt.

A magas előremenő hőmérséklet nem bizonyít önmagában magasabb tüzelőanyag-hatásfokot. Azt igazolja, hogy a rendszer nagy hőteljesítményt tudott koncentráltan a fűtési körbe juttatni. A jó teljes energiahasznosítás mérnöki alapját a következő elemek együttese adta: motorhűtési hő visszanyerése, kipufogóhő visszanyerése, nagy hőcserélő felület, stabil munkapont, korlátozott villamos melléktermelés, nagy termikus tárolókapacitás, ciklikus üzem.

### 9/A.12. A motoroldali és az épületoldali optimum eltérése

- **Motoroldali optimum:** a gép stabil és kedvező működési pontja (400–410 fordulat/perc, stabil égés, alacsony zaj, egyenletes járás, jól szabályozható hűtés).
- **Épületoldali optimum:** az a pillanatnyi hőteljesítmény, amely éppen fedezte az épület hőveszteségét — ez kisebb volt.

A két optimum közötti különbséget a puffertartály és a termikus tömeg hidalta át. A motor rövid ideig az optimális saját munkapontján működött, az épület pedig hosszabb idő alatt, a hőtárolóból kapta meg a szükséges átlagos teljesítményt.

**Ez a rendszer egyik legfontosabb működési elve.**

### 9/A.13. A szükséges hőelnyelő kapacitás

A prototípus a rendelkezésre álló fűtési hálózatot és különösen a közösségi helyiséget gyorsan túlmelegítette. Ez arra utal, hogy a motor minimális stabil hőteljesítménye meghaladta az adott időpontban rendelkezésre álló folyamatos hőelnyelő kapacitást. A folyamatos üzemhez nagyobb fűtött terület, nagyobb puffertároló, több folyamatos hőigényű épületrész, fólia- vagy üvegház, használati melegvíz-termelés vagy technológiai hőfelhasználás kellett volna.

A mérnökileg védhető állítás:

> „A prototípus minimális stabil hőteljesítménye az adott közösségi helyiség pillanatnyi hőigényét többszörösen meghaladta. A berendezés folyamatos üzeméhez lényegesen nagyobb állandó hőelnyelő kapacitásra lett volna szükség.”

### 9/A.14. A hőtárolás és a hatásfok kapcsolata

A nagy termikus tehetetlenség önmagában nem növeli a tüzelőanyagból kinyerhető energia mennyiségét. A hőtároló rendszer azonban javíthatja a gyakorlati, szezonális működést, mert csökkenti az instabil részterhelési időszakokat, lehetővé teszi az optimális motorfordulaton történő üzemet, csökkenti a túl gyakori indításokat, mérsékli a hőmérséklet-ingadozást, és időben szétválasztja a hőtermelést és a hőfelhasználást.

Ezért a prototípus megítélésénél két külön mutatót kell használni: a **pillanatnyi összesített hatásfokot** és az **időszakos vagy szezonális gázfelhasználást**. Ezek mérési adatai hiányában a rövid hőtartási ciklusok jó gyakorlati működést jeleznek, de egzakt szezonális hatásfokot nem bizonyítanak.

### 9/A.15. Korrigált mérnöki következtetés

A prototípus működését nem helyes kizárólag a hideg állapotból történő első felfűtés alapján értékelni. A rendszer lényegi működése: a gázmotor stabil munkapontban rövid idő alatt jelentős hőteljesítményt termelt; a hő a fűtési rendszerbe került; a puffer, a vízhálózat, a radiátorok és az épületszerkezet nagy mennyiségű energiát tárolt; a motor leállítása után a fűtés hosszabb ideig folytatódott; a hőntartáshoz egyes időszakokban óránként csak néhány vagy körülbelül tíz perc motorüzemre volt szükség.

Ez a működés nem bizonyít többszörös termodinamikai hatásfokot, de igazolja a nagy termikus tárolásra épülő, ciklikus rendszer gyakorlati életképességét. A prototípus folyamatos üzeméhez nagyobb hőelnyelő oldal — például nagyobb ingatlan, műhely-, raktár- vagy fóliaházi rendszer — lett volna megfelelőbb.

## 10. Megfigyelt természetes validációs jelenségek

### 10.1. Helyiség-túlmelegedés

Egy üzemi próba során a 80 m²-nél nagyobb közösségi tér hőmérséklete emberileg nehezen elviselhető szintre emelkedett, és a helyiségben tartózkodók kérték a rendszer leállítását. Ez nem számszerű hőmérsékletmérés, de erős kvalitatív bizonyíték arra, hogy a radiátoros kör rövid idő alatt nagy hőteljesítményt adott le.

### 10.2. Radiátorérintési sérülés

A radiátor felületének kézi ellenőrzésekor az érintés égési sérülést vagy legalább azonnali, erős termikus sérülést okozott. Ebből egzakt radiátor-hőmérséklet nem vezethető le, de a megfigyelés igazolja, hogy a radiátor felülete nem egyszerűen meleg, hanem veszélyesen forró volt.

### 10.3. Új radiátorok festékkárosodása

A fűtési rendszert közvetlenül a kísérleti időszak előtt felújították, a radiátorok újonnan felszerelt állapotban voltak. Nagy hőterhelésnél a festék a belépőcsonkok környezetében felrepedt, egyes helyeken levált, és a radiátorlemez helyileg deformálódott vagy kidudorodott.

A festékkárosodás önmagában nem alkalmas pontos vízhőmérséklet meghatározására, de a többi megfigyeléssel együtt jelentős tapasztalati bizonyíték. A korábbi tanulmányban szereplő „legalább 95 °C-os vízhőmérséklet” ezért túlzottan pontos állítás volt. A helyes megállapítás:

> „A radiátorok belépő szakaszán rendkívül magas, műszeresen nem dokumentált helyi hőmérséklet és termikus-mechanikai igénybevétel alakult ki.”

### 10.4. Alacsony zaj

A motor nyitott térben, külön hangszigetelő burkolat nélkül működött, és a működés rendkívül csendes volt. Megfigyelési adatként rögzíthető, hogy egy csecsemő a motortól hozzávetőleg egyméteres távolságban, hordozóban zavartalanul aludt. Ez nem szabványos decibelmérés.

A csendes működést valószínűleg együttesen okozta a kb. 400 fordulat/perces rendkívül alacsony fordulatszám, a négyhengeres kialakítás, a nagy lendítőtömeg, az egyenletes mechanikai terhelés, a stabil gázüzem és a magasabb frekvenciájú égési és mechanikai zajok hiánya.

## 11. Villamosenergia-termelés

### 11.1. Igazolt terhelés

A 48 voltos akkumulátoros rendszerből időszakosan körülbelül 1 kW teljesítményt vettünk ki. Ehhez 48 V-on I = 1000 W / 48 V ≈ 20,8 A áram tartozik — ez a nagyságrend a generátor, az egyenirányító és az akkumulátorrendszer számára reális.

### 11.2. A 2 kW-os becslés

A korábbi tanulmány körülbelül 2 kW villamos teljesítménnyel számolt. Ehhez 48 V-on ≈ 41,7 A kellene. Ez gépészetileg lehetséges áramérték egy targoncából származó 48 voltos generátornál, de nem áll rendelkezésre olyan hitelesített mérési jegyzőkönyv, amely igazolná a folyamatos 41–42 amperes kimenetet. Ezért a helyes besorolás:

- igazoltan kezelt terhelés: körülbelül 1 kW időszakosan;
- valószínű villamos teljesítménytartomány: körülbelül 1–2 kW;
- 2 kW: felső becslés, nem laboratóriumi mérési eredmény.

### 11.3. Villamos hatásfok

1 kW kimenetnél η_el ≈ 1 / 28,33 ≈ 3,5%; 2 kW kimenetnél η_el ≈ 7,1%. Mindkét érték alacsony a hagyományos villamosenergia-termelő gázmotorokhoz képest, ez azonban összhangban áll a rendszer céljával: a mechanikai és villamos kimenetet szándékosan másodlagosnak kezeltük a hőtermeléshez képest.

## 12. Becsült hőteljesítmény és összhatásfok

### 12.1. Mi számítható biztosan?

Biztosan vagy jó közelítéssel ismert: a kb. 28,3 kW tüzelőanyag-bemenet; az igazoltan időszakos kb. 1 kW (becslés szerint legfeljebb kb. 2 kW) villamos kimenet; hogy a rendszer hűtőköri és kipufogóoldali hőt is hasznosított; hogy a motor és a fűtési rendszer tartósan működött; és hogy jelentős hőmennyiség jutott a radiátoros körbe.

Nem ismert: az előremenő és visszatérő vízhőmérséklet, a tényleges víztömegáram, a kipufogógáz tömegárama, a hőcserélő belépő és kilépő gázhőmérséklete, a környezeti veszteség, valamint a generátor és a DC–DC átalakító pontos hatásfoka. Ezért a hasznos hőteljesítmény nem határozható meg egyetlen egzakt számmal.

### 12.2. Konzervatív energiamérleg

```
P_be = P_el + Q_hasznos + P_veszteség
```

| Teljes hasznosítás | Hasznos villamos + hő | Becsült hasznos hő (1–2 kW villamos mellett) |
|---|---|---|
| 70% | ≈ 19,83 kW | ≈ 17,8–18,8 kW |
| 80% | ≈ 22,66 kW | ≈ 20,7–21,7 kW |
| 85% | ≈ 24,08 kW | ≈ 22,1–23,1 kW |
| 90% | ≈ 25,50 kW | ≈ 23,5–24,5 kW |

A hagyományos CHP-rendszereknél a teljes hasznosítás gyakran 60–80% körüli tartományban van. A jelen prototípus ettől eltérő, kifejezetten hőtermelésre hangolt rendszer volt; a nagy felületű hőcserélő, a motorhűtés teljes integrációja és a nem nyilvános saját konstrukciós megoldás miatt ennél magasabb hasznosítás elvileg lehetséges. A 95,3%-os érték azonban utólag nem bizonyítható.

### 12.3. A korábbi 25 kW-os hőbecslés értékelése

Ha P_be = 28,33 kW, P_el = 2 kW és Q_hő = 25 kW, akkor η_össz = (2 + 25) / 28,33 ≈ 95,3%. Ez matematikailag helyes, de mérnöki státusza: nem mért eredmény, nem bizonyított tényleges hatásfok, hanem felső becslési forgatókönyv. A tanulmány helyes állítása:

> „A prototípus hasznos hőteljesítménye valószínűleg 18–24 kW közötti tartományban lehetett. A korábbi 25 kW-os érték lehetséges felső becslés, amelyhez körülbelül 95%-os összesített energiahasznosítás tartozna. Ennek közvetlen műszeres igazolása nem történt meg.”

### 12.4. Mi igazolja mégis a magas hasznosítást?

A magas hőhasznosítást az alábbi együttes körülmények támogatják: a motor extrém alacsony mechanikai hatásfoka; a motorhűtési hő teljes fűtési integrációja; a kipufogó hőjének visszanyerése; jelentősen túlméretezett hőcserélő; alacsony gázoldali fojtás; tartósan stabil motorhőmérséklet; nagy fűtött komplexum; 1000 literes puffer; rendkívül forró radiátorok; helyiségtúlmelegedés; két teljes téli szezon valós üzeme. Ezek nem helyettesítik a kalorimetrikus mérést, de erős tapasztalati validációt jelentenek.

## 13. Üzemeltetési idő és tartósság

A prototípust két téli szezonban használtuk. Az első fűtési időszak hozzávetőleg október végétől márciusig tartott; a következő télen a működést megismételtük. Az egyes üzemmenetek néhány órás, többórás és több tíz órás folyamatos működést is magukban foglaltak. A rendszer nem egyszeri demonstráció vagy néhány perces próba volt.

A rendszert végül nem műszaki meghibásodás miatt bontottuk el. A további fejlesztésre és hasznosításra akkor nem mutatkozott külső érdeklődés.

## 14. Műszaki minősítés

| Kategória | Tartalom |
|---|---|
| **Mért** | kb. 3 m³/h földgázfogyasztás hitelesített gázórával; 400–410 fordulat/perc lézeres fordulatszámmérővel; 48 voltos villamos rendszer; 2 bar fölötti, közel 3 barig emelkedő fűtési rendszernyomás |
| **Megfigyelt** | két téli szezonon át történő működés; néhány órától több tíz óráig tartó folyamatos üzem; stabil motorhőmérséklet; rendkívül alacsony zaj; 500 fordulat/perc fölött vörösen izzó kipufogócsonk; részben megolvadt hőcserélő-csatlakozás; veszélyesen forró radiátorok; radiátorfesték repedése és leválása; lokális radiátorlemez-deformáció; a közösségi helyiség jelentős túlmelegedése |
| **Utólag számítható** | kb. 28,3 kW tüzelőanyag-bemenet; kb. 102 MJ bevitt energia óránként; 1 kW-nál kb. 20,8 A, 2 kW-nál kb. 41,7 A; 1000 liter víz elméleti, veszteségmentes 24,4 °C-os felmelegítése egy óra alatt |
| **Becsült** | kb. 1–2 kW villamos teljesítmény; kb. 18–24 kW hasznos hőteljesítmény; kb. 70–90% teljes hasznosítás; legalább 100 méteres, feltehetően több száz méteres csőhálózat |
| **Utólag nem igazolható** | egzakt 95,3%-os teljes hatásfok; pontos radiátor-vízhőmérséklet; pontos kipufogógáz-hőmérséklet; teljes pillanatnyi víztömegáram; a hőcserélő tényleges hőátadási teljesítménye; a generátor folyamatos 2 kW-os nettó kimenete |

### Végső műszaki következtetés

A rendelkezésre álló adatok alapján a prototípus működése termodinamikailag lehetséges, gépészetileg konzisztens, tapasztalatilag igazolt, több hónapos üzemben validált és energetikai szempontból életszerű. A berendezés helyes besorolása:

> „Műhelyalapú, funkcionális újrahasznosítással létrehozott, extrém alacsony fordulatszámú, hőtermelésre optimalizált gázmotoros kapcsolt hő- és villamosenergia-termelő kísérleti prototípus.”

A rendszer nem tekinthető teljes körűen műszerezett laboratóriumi mintadarabnak, de nem is puszta elméleti koncepció. Fizikailag megépített, ismételten működtetett és két téli szezonban tényleges fűtési feladatot ellátó berendezés volt.

## 15. Rekonstrukciós lehetőség

A rendszer mai eszközökkel újra megépíthető lenne. Egy korszerű rekonstrukciónál szükséges mérési rendszer: hitelesített gázmennyiségmérés; gáznyomás- és hőmérsékletmérés; előremenő és visszatérő vízhőmérséklet; motorhűtőköri és radiátoros köri térfogatáram; kipufogógáz belépő és kilépő hőmérséklet; kipufogóoldali nyomásesés; füstgáz O₂-, CO₂-, CO-, NOₓ- és szénhidrogén-tartalom; motorfordulatszám; tengelynyomaték; generátorfeszültség és áram; a DC–DC konverter bemeneti és kimeneti teljesítménye; a puffertartály réteghőmérséklete több magasságban; a környezeti hőveszteség becslése.

```
Q̇ = ṁ × c_p × (T_előremenő − T_visszatérő)
η_össz = (P_el,nettó + Q̇_hasznos) / P_üzemanyag
```

Ezzel a korabeli prototípus ma már pontosan mérhető és reprodukálható mérnöki rendszerré alakítható lenne.

## 16. A szellemi érték és a nyilvánosság határa

A prototípus értéke nem pusztán abban állt, hogy egy régi gázmotort egy hőcserélőhöz kapcsoltak. A fő értéket az a nem nyilvános saját műszaki megoldás képviseli, amely meghatározta az extrém alacsony fordulatszámú stabil égést, a hőtermelés és a mechanikai kimenet arányát, a motor üzemi hőmérsékletének szabályozását, a kipufogóoldali hő hatékony kivételét, a hőcserélő és a két folyadékkör együttműködését, valamint a rendszer összesített működési optimumát.

A jelen dokumentum ennek a megoldásnak a létezését és funkcióját rögzíti, de a pontos konstrukciót nem közli. A nyilvános rész célja a prototípus történeti dokumentálása, a működőképesség mérnöki ellenőrzése, az energiamérleg életszerűségének igazolása és a fejlesztési elv bemutatása. A nem nyilvános rész tartalmazza azt a know-how-t, amely nélkül a rendszer hasonló hatásfoka és stabil működése nem feltétlenül reprodukálható.

## 17. Későbbi offline AI-integráció

Az offline AI-rendszer nem része a korabeli kísérlet bizonyított működésének; ez egy később hozzáadott fejlesztési irány. A gázmotoros energiaközpont elvileg alkalmas lehetne folyamatos alap villamos energia előállítására, akkumulátoros energiatárolás töltésére, helyi szerverinfrastruktúra hő- és villamosenergia-ellátására, és a szerverek hulladékhőjének további fűtési hasznosítására.

Egy nagy, több GPU-s offline AI-klaszter azonban nem táplálható közvetlenül a korabeli 1–2 kW-os generátorkimenetről teljes terhelésen. A nagy klasztert külön energetikai alrendszerként kell kezelni (nagy kapacitású akkumulátoros puffer, több párhuzamos energiaforrás, inverteres és DC-sínes energiaelosztás, szakaszos nagy teljesítményű futtatás, a gázmotoros egység mint részleges töltő- és hőtermelő modul). Ennek részletes tervezése külön mérnöki tanulmány tárgya, és nem keverhető össze a korabeli prototípus mért eredményeivel.

## Összegzés

A kísérleti rendszer alapgondolata az volt, hogy egy hagyományos Ottó-motor korlátozott mechanikai hatásfokát ne hátrányként, hanem hőtermelési lehetőségként kezeljük. A megoldás:

- megmentett egy működőképes motort és generátort a megsemmisítéstől;
- új funkcióba helyezte a donorberendezés részegységeit;
- alacsony fordulatszámú gázüzemmel stabil hőforrást hozott létre;
- a motorhűtés és a kipufogó hőjét egyaránt hasznosította;
- egy körülbelül 450 m²-es komplexum fűtésében vett részt;
- villamos melléktermelést biztosított;
- két teljes téli szezonban működött.

A 3 m³/h földgázfogyasztásból számítható körülbelül 28,3 kW bemenő teljesítmény összhangban áll a megfigyelt nagy hőtermeléssel. A valószínű hasznos hőteljesítmény konzervatívan körülbelül 18–24 kW tartományba helyezhető; a villamos kimenet körülbelül 1–2 kW lehetett. A korábban megadott 25 kW hőteljesítmény és 95,3%-os összhatásfok nem zárható ki teljes bizonyossággal, de közvetlen mérési adatok hiányában nem kezelhető igazolt eredményként.

A prototípus valódi mérnöki értéke három elem együttese:

1. funkcionális ipari újrahasznosítás;
2. szokatlan, hőtermelésre optimalizált motorüzem;
3. a nem nyilvános saját konstrukciós megoldás, amely a kedvező termikus működést és stabilitást lehetővé tette.

**A rendszer a leírt formában működhetett, és a több hónapos, két téli szezonban végzett tényleges üzem alapján működött is.**
