**Language:** [Magyar](README.md) | [English](README.en.md)

# Mérnöki esettanulmányok / Engineering Case Studies

**Almási Andor** — gyakorlati energetikai és teljesítményelektronikai fejlesztések dokumentációja: hőhasznosítás, energiatárolás, funkcionális újrahasznosítás.

> **English summary below.**

## Miről szól ez a repó?

Ezek a dokumentumok valós, műhelyben megépített vagy előkészített rendszereket írnak le. Közös bennük a szemlélet: először azt kell megnézni, mi áll már rendelkezésre, és csak azt kell újonnan beszerezni, ami valóban nem helyettesíthető. A másik közös elv a bizonyítéki fegyelem: minden dokumentum külön kezeli a **mért**, a **megfigyelt**, az **utólag számított** és a **becsült** adatokat, és kimondja, mi nem igazolható utólag.

## Tartalom

| # | Dokumentum | Röviden |
|---|---|---|
| 01 | [Gázmotoros energiaközpont — mérnöki esettanulmány](01_Gazmotoros_energiakozpont_esettanulmany.md) | Kiégett targoncából kimentett 1,6 literes motor, dugattyús gázkazánként üzemeltetve 400 fordulat/perc körül. Két fűtési szezon, kb. 450 m² fűtött terület, kb. 28 kW tüzelőanyag-bemenet, becsülten 18–24 kW hasznos hő. |
| 02 | [200 kWh-s LiFePO4 energiatároló — felügyeleti architektúra](02_200kWh_LiFePO4_felugyeleti_architektura.md) | Rétegzett adatgyűjtési és felügyeleti terv (cella → BMS → gateway → HMI → külső világ), interfész-logika és 120S5P cellaszámítás. |

## Mi nincs benne — szándékosan

A dokumentumok a működési elvet, az energiamérleget és a felépítést mutatják be. A rendszerek fő szellemi értékét képviselő saját konstrukciós megoldások, a kalkulációk, készletadatok és üzleti részletek **nem** nyilvánosak.

## Kapcsolódó

- AI-munkafolyamat és validációs portfólió: [AI-Workflow-Validation-Portfolio](https://github.com/hyperbetteri/AI-Workflow-Validation-Portfolio)
- AI-motor megfigyelések: [AI-Engine-Observations](https://github.com/hyperbetteri/AI-Engine-Observations)

---

## English summary

Documentation of practical energy and power-electronics work, built in a workshop rather than a lab:

- **Gas-engine heat and power centre (case study)** — a 1.6-litre four-cylinder engine and 48 V generator rescued from a fire-damaged forklift, run deliberately at about 400 rpm as a "piston gas boiler". It heated roughly 450 m² for two full winter seasons. Measured gas use of about 3 m³/h corresponds to about 28 kW fuel input; useful heat is conservatively estimated at 18–24 kW. The study strictly separates measured, observed, calculated and estimated values, and keeps the key proprietary design element undisclosed.
- **200 kWh LiFePO4 storage — monitoring architecture** — a layered data-acquisition and supervision design (cell → BMS → gateway/PLC → HMI → external systems) with interface logic and a 120S5P cell calculation.

The documents are in Hungarian. Proprietary design details, cost calculations, inventory and business data are deliberately omitted.

---

© 2026 Almási Andor. Minden jog fenntartva. Forrásmegjelöléssel szabadon idézhető. / All rights reserved. Quotation with attribution is welcome.
