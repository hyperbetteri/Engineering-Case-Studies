**Language:** [Magyar](README.md) | [English](README.en.md)

# Engineering Case Studies / Mérnöki esettanulmányok

**Almási Andor** — documentation of practical energy and power-electronics developments: heat recovery, energy storage, functional reuse.

## What is this repository about?

These documents describe real systems that were built, or prepared for building, in a workshop. They share a common approach: first look at what is already available, and only newly acquire what genuinely cannot be substituted. The other shared principle is evidential discipline: every document treats **measured**, **observed**, **retrospectively calculated** and **estimated** data separately, and states explicitly what cannot be verified after the fact.

## Contents

| # | Document | In brief |
|---|---|---|
| 01 | [Gas-engine energy centre — engineering case study](01_Gazmotoros_energiakozpont_esettanulmany.en.md) | A 1.6-litre engine rescued from a fire-damaged forklift, operated as a piston gas boiler at around 400 rpm. Two heating seasons, approx. 450 m² heated area, approx. 28 kW fuel input, an estimated 18–24 kW useful heat. |
| 02 | [200 kWh LiFePO4 energy storage — monitoring architecture](02_200kWh_LiFePO4_felugyeleti_architektura.en.md) | Layered data-acquisition and monitoring design (cell → BMS → gateway → HMI → external world), interface logic and a 120S5P cell calculation. |

## What is not included — deliberately

The documents present the operating principle, the energy balance and the design. The proprietary design solutions that represent the main intellectual value of the systems, as well as the calculations, inventory data and business details, are **not** public.

## Related

- AI workflow and validation portfolio: [AI-Workflow-Validation-Portfolio](https://github.com/hyperbetteri/AI-Workflow-Validation-Portfolio)
- AI engine observations: [AI-Engine-Observations](https://github.com/hyperbetteri/AI-Engine-Observations)
- Legal AI framework (overview): [LEGAL-RQV-Overview](https://github.com/hyperbetteri/LEGAL-RQV-Overview)
- Lunar recycling concept studies: [Lunar-Recycling-and-Terminator-Lab](https://github.com/hyperbetteri/Lunar-Recycling-and-Terminator-Lab)

---

## Summary

Documentation of practical energy and power-electronics work, built in a workshop rather than a lab:

- **Gas-engine heat and power centre (case study)** — a 1.6-litre four-cylinder engine and 48 V generator rescued from a fire-damaged forklift, run deliberately at about 400 rpm as a "piston gas boiler". It heated roughly 450 m² for two full winter seasons. Measured gas use of about 3 m³/h corresponds to about 28 kW fuel input; useful heat is conservatively estimated at 18–24 kW. The study strictly separates measured, observed, calculated and estimated values, and keeps the key proprietary design element undisclosed.
- **200 kWh LiFePO4 storage — monitoring architecture** — a layered data-acquisition and supervision design (cell → BMS → gateway/PLC → HMI → external systems) with interface logic and a 120S5P cell calculation.

The original documents are written in Hungarian; the full English translations are linked in the Contents table above. Proprietary design details, cost calculations, inventory and business data are deliberately omitted.

---

© 2026 Almási Andor. All rights reserved. Quotation with attribution is welcome.
