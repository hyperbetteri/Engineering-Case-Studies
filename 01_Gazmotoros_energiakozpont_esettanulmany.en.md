**Language:** [Magyar](01_Gazmotoros_energiakozpont_esettanulmany.md) | [English](01_Gazmotoros_energiakozpont_esettanulmany.en.md)

# Experimental Implementation of a Gas-Fired, Internal-Combustion-Engine Energy Centre Optimised for Heat Production

**Engineering case study**

Author: Almási Andor · Canonical technical version: 5 August 2026 · Public version

> **Publication note.** This version contains the canonical technical case study. The exact operation, design and control principle of the proprietary design solution, which represents the main intellectual value of the system, are not public (see sections 7.5 and 16). The documentation and contact appendix is not part of the public version.

## Executive summary

This case study documents a gas-fired combined heat and power prototype built in a workshop through functional reuse.

The system was based on a 1.6-litre, four-cylinder Otto (spark-ignition) engine of Volkswagen Polo origin, together with its 48-volt electric generator, both rescued from a gas-fuelled Still forklift with electric drive.

The internal wiring harness of the donor forklift had been severely damaged by an earlier electrical cable and wiring fire. The vehicle was never repaired, but the internal combustion engine, the generator and several associated mechanical subassemblies remained intact and operational. Instead of being dismantled or melted down, these subassemblies were given a second functional life cycle in a new energy system.

The aim of the development was not to maximise the mechanical output of the Otto engine. The opposite was done: the engine was deliberately operated at an extremely low speed, at which the overwhelming majority of the fuel energy appeared as heat.

The concept in brief:

- we did not try to turn the Otto engine, which has an inherently moderate mechanical efficiency, into a high-output prime mover;
- the share of mechanical energy was deliberately kept low;
- the heat generated in the engine block, the coolant and the exhaust gas was recovered;
- the unit was used primarily as a piston gas boiler;
- electricity was a secondary but useful by-product.

Measured with a certified (calibrated) gas meter, the system consumed approximately 3 m³ of natural gas per hour. The stable operating speed was continuously checked with a laser tachometer. The optimum range was 350–450 rpm, with typical operation at 400–410 rpm.

The prototype operated for two full winter heating seasons. Individual runs lasted from a few hours to several tens of hours. The system heated a complex of workshop, warehouse and community buildings with a total floor area of approximately 450 m², via a permanently connected buffer tank of about 1 m³ and an extensive radiator pipe network.

The power measurements of the time did not reach the level of instrumentation of a present-day laboratory test. For this reason, the document clearly separates:

- directly measured data;
- phenomena observed during extended operation;
- values that can be calculated retrospectively;
- estimated parameters;
- and the non-public design solutions.

Based on the available data, the operation of the prototype is thermodynamically and mechanically consistent. The exact overall efficiency cannot be determined retrospectively, but the high heat output, the stable long-term operation and the combined utilisation of the engine's cooling-circuit and exhaust-side heat can be substantiated from an engineering standpoint.

## 2. Conceptual basis of the development

### 2.1 Functional reuse

One of the primary principles of the development was that the system should not be built from predefined, newly purchased components. The design process started from the following questions:

- what working subassemblies are available in the surroundings;
- what original function they were made for;
- in what other function they can be used;
- what minimal modification is needed to integrate them into the new system.

The approach is summed up by a family saying:

> "You don't have to buy a whole cow just to drink a glass of milk."

In technical terms this did not mean makeshift or careless workmanship, but that the functional potential of the available resources must be recognised first. Only what genuinely cannot be replaced by an existing item needs to be newly purchased or manufactured.

The engine and generator from the donor forklift were used in line with this value-salvaging logic. Both main units were in faultless working order, even though the original vehicle had already been earmarked for scrapping because of the wiring fire.

### 2.2 Workshop-based development

The prototype was not built within a formal research and development programme, not in a laboratory, and not on the basis of complete prior engineering documentation.

The developers had:

- practical mechanical and electrical knowledge;
- assembly and workshop experience;
- working technical intuition;
- access to a variety of industrial components and tools.

However, the following were not available:

- a complete calorimetric measurement system;
- a calibrated torque-measuring dynamometer;
- continuous flue-gas analysis;
- temperature and volumetric flow measurement installed at every point of the heating circuits;
- a computational fluid dynamics model prepared in advance.

The design evolved iteratively: selection of available components → mechanical fitting → trial run → observation → adjustment and modification → repeated extended operational testing.

This method is not the same as standard industrial product development, but it was suitable for demonstrating that the underlying principle can be realised as a system that works in practice.

## 3. The donor unit and the main subassemblies

### 3.1 The donor Still forklift

The donor unit was a gas-fuelled Still forklift with electric drive. In this forklift's operating principle, the internal combustion engine drove a 48-volt generator that supplied power to the vehicle's electrical system.

The forklift's internal wiring had previously burnt out. The damage did not materially affect:

- the internal combustion engine of Volkswagen origin;
- the 48-volt generator;
- the main mechanical units;
- several associated control and drive components.

The exact year of manufacture of the donor unit is not known. At the time of the experiment the engine was already an older design, but it had remained in mechanically serviceable condition.

### 3.2 Internal combustion engine

Main data of the prime mover:

| Characteristic | Data |
|---|---|
| Origin | Volkswagen Polo design |
| Displacement | approximately 1.6 litres |
| Number of cylinders | four |
| Operating principle | four-stroke Otto engine |
| Original fuel | petrol, or a version suitable for gas operation |
| Experimental fuel | first LPG (propane-butane), later mains natural gas |
| Mixture formation | carburettor system |
| Gas introduction | on the air side of the carburettor |
| Ignition | contact-breaker-based, partly mechanical and partly electronic system, presumably with Hall-effect sensor triggering |

The exact type of the ignition system cannot be identified retrospectively with complete certainty. What can be reliably reconstructed is that spark generation did not rely solely on conventional mechanical distribution; an electronic switching stage was also involved.

### 3.3 Generator and electrical connection

The 48-volt generator originally belonging to the engine was retained. The generator:

- was directly mechanically coupled to the engine;
- operated without any gearing;
- rotated at a speed of the same order as the engine crankshaft;
- delivered a pulsating DC output;
- was connected to charge a lead-acid battery bank;
- at times also supplied an electrical load of the order of about 1 kW.

A Graetz bridge (bridge rectifier), rectifier diodes and a DC-link buffer capacitor of several tens of thousands of microfarads were connected to the electrical output. The buffer capacitor served to:

- smooth the pulsating output of the generator;
- provide a more stable input supply to the DC–DC converter;
- reduce momentary voltage fluctuations;
- partly cover the transient demand of switched loads.

Initially the system was harder to start until the high-capacitance capacitor had charged up. This is consistent with the capacitor drawing a high inrush current for a short time when empty.

### 3.4 Flywheel and shaft coupling

A separately bearing-mounted flywheel with a mass of approximately 80 kg was located between the engine crankshaft and the generator. Elements of the mechanical connection:

- bearing-mounted flywheel;
- Hardy disc or a similar flexible coupling element;
- jaw (claw) coupling;
- minimal lathe-machined fitting;
- direct drive without gearing.

The role of the flywheel was fundamental. Because of the extremely low speed, significant angular-velocity fluctuations could have developed between the power strokes of the individual cylinders. The flywheel, with its high moment of inertia:

- stored energy during the power stroke;
- returned the energy during the compression and exhaust strokes;
- made crankshaft rotation more uniform;
- reduced the risk of stalling;
- moderated the impulsive loading of the drivetrain;
- stabilised the generator voltage;
- reduced vibration and noise.

The exact diameter and mass distribution of the flywheel are not documented. For this reason the stored rotational energy cannot be calculated reliably, but given a mass of about 80 kg the stabilising effect may have been considerable.

## 4. Thermodynamic logic of the concept

### 4.1 The aim was not to maximise mechanical efficiency

When a conventional internal combustion engine is developed, the aim is usually for as large a share of the fuel energy as possible to appear as useful shaft power. This project applied a different objective function. The aim was that:

- the engine should produce only as much mechanical power as is needed for its own operation, for driving the generator and for a stable load;
- a larger share of the fuel energy should appear as heat in the engine block and in the exhaust gas;
- this heat should be transferred to the heating system in the highest possible proportion.

The deliberate reduction of mechanical efficiency therefore did not mean a reduction in overall energy utilisation. The aim of the system was to change the distribution of the energy output: a smaller electrical and mechanical share, a larger recoverable heat share.

### 4.2 Internal-combustion piston gas boiler

Functionally, the system can be regarded as a gas boiler in which combustion took place not in a continuous combustion chamber but in cylinders, with periodic compression and ignition. In this operating state the engine simultaneously provided:

- intake of the gas–air mixture;
- compression of the mixture;
- controlled timing of combustion;
- heat transfer to the engine block and the coolant;
- delivery of the hot combustion products to the exhaust heat exchanger;
- limited mechanical and electrical co-generation.

### 4.3 Classification as combined heat and power

Technically, the system can be regarded as a combined heat and power (CHP) prototype. The general definition of total CHP efficiency:

```
η_total = (P_el + Q_useful heat) / P_fuel
```

where P_el is the net useful electrical power, Q_useful heat is the heat output actually utilised, and P_fuel is the power input supplied by the fuel.

In CHP systems, heat can be recovered from the engine's exhaust gas, its coolant and, in some cases, its lubricating oil. This is not a unique or physically anomalous procedure, but a well-known basic principle of reciprocating-engine combined heat and power. According to the EPA technology catalogue, heat from a reciprocating engine can be recovered from several sources, including the exhaust and the jacket water.

The distinctive feature of the prototype at the time was that it applied this principle at an unusually low speed and in an operating state specifically optimised for heat production.

## 5. Fuel supply

### 5.1 Initial trials with LPG

The first trials of the system were carried out with LPG (propane-butane). An earlier summary stated an LPG consumption of 2 m³/h. Based on the present recollection, this figure cannot be treated as measured data with the same certainty as the natural gas consumption. Therefore the LPG consumption value can be used only as a contemporary estimate or preliminary trial data.

### 5.2 Natural gas operation

Later, long-term operation was on mains natural gas. Gas consumption was measured with a separately installed, certified gas meter.

Measured natural gas consumption: **V̇gas ≈ 3 m³/h**

Calculating with a lower heating value of 34 MJ/m³:

```
P_in = 3 m³/h × 34 MJ/m³ = 102 MJ/h
1 kWh = 3.6 MJ  →  P_in = 102 / 3.6 ≈ 28.33 kW
```

The consumption of 3 m³/h therefore corresponded to a fuel-side power of approximately 28.3 kW. The actual heating value of natural gas may vary depending on the grid gas composition and the billing reference conditions. For this reason, as an engineering estimate, it is advisable to assume an input power of about 27–30 kW.

## 6. Speed and operating state

### 6.1 Measured operating speed

The engine speed was continuously checked with a laser tachometer.

- Measured typical operating value: **400–410 rpm**
- Empirically usable range: **350–450 rpm**

The speed was held stable by mechanical governing.

### 6.2 The range above 500 rpm

When the engine speed was raised above 500 rpm:

- the cast exhaust manifold began to glow red;
- the pipe connected to the heat exchanger was subjected to extreme thermal load;
- the connection partly melted or broke off;
- the pipe later had to be welded back on.

This was not a normal operating range. The exact temperature of the red glow is not known. However, the observation clearly indicates that above 500 rpm the exhaust-side thermal load rose rapidly and to an unacceptable degree.

The setting of around 400–410 rpm was therefore not an arbitrary choice but the result of empirical optimisation: stable combustion, manageable thermal load, adequate generator loading, low noise, smooth running, longer-term operational reliability.

## 7. Heat recovery system

### 7.1 Heat sources

The system utilised two main heat sources: the engine cooling heat and the heat content of the exhaust gas. In reciprocating-engine CHP systems, combined heat recovery from the jacket water and the exhaust gas is a technically well-known solution. The engine exhaust gas is at a higher temperature, while the cooling circuit provides a more stable, lower-temperature heat source.

### 7.2 Plate heat exchanger

The prototype used a professional plate heat exchanger in new condition, with a nominal capacity of approximately 400 kW, probably manufactured by Alfa Laval. The nominal rating of 400 kW does not represent the actual heat output of the engine.

The main reasons for choosing this heat exchanger were that:

- the connections of the smaller unit available were inadequate;
- the large unit had inlet and outlet connections larger than 1 inch;
- an adequate cross-section was needed to pass the flue gas through;
- excessive exhaust back-pressure had to be avoided;
- a smaller flow cross-section could have impeded the discharge of the flue gas;
- throttling could have impaired combustion and engine stability.

For gas-side heat exchangers, low pressure loss is indeed a decisive design consideration. The actual choice of heat exchanger was therefore determined not by a 400 kW heat demand but by the available port size, flow cross-section and low gas-side resistance.

### 7.3 Separation of media

The flue gas did not mix with the heating water or the engine coolant. In the separate channel systems of the heat exchanger, the hot flue gas flowed on one side and the liquid circuit on the other. The exact internal plate arrangement and channel configuration cannot be reconstructed retrospectively. During installation, however, care was deliberately taken that the sides were not cross-connected and that the media did not mix.

### 7.4 Engine cooling circuit

The engine's own liquid cooling system was also connected to the heat recovery system. Engine cooling had a dual function: keeping the engine at a stable operating temperature and using the heat generated in the engine block for space heating.

Based on several months of repeated winter operation, heat removal was adequate on a sustained basis. This was not merely a short demonstration: the engine operated in uninterrupted runs of a few hours as well as several tens of hours.

### 7.5 Non-public design solution

The high heat utilisation of the system was not achieved solely through the use of the large heat exchanger. The overall design included a proprietary technical solution or group of solutions that:

- determined the actual thermal operating state of the engine;
- influenced the relationship between combustion, speed and heat removal;
- enabled favourable utilisation of the cooling-circuit and exhaust-side energy;
- represents the main intellectual and technical value of the system.

Its exact mode of operation, geometric design, circuit arrangement and control principle are not public. The study therefore describes only the external energy balance and the documentable operation of the system. The key proprietary solution is not detailed, and its place must not be filled with assumed or retrospectively invented explanations.

## 8. Heating system

### 8.1 Heated complex

The system heated a large building complex in Debrecen. The complex consisted of three main parts: a workshop, a large warehouse, and a kitchen–dining–community area.

The total heated floor area was approximately **450 m²**. The exact value may have differed by a few square metres, but the order of magnitude of 450 m² is realistic.

### 8.2 Kitchen–dining–community area

The best-documented individual room:

- floor area: at least 80 m²;
- ceiling height: about 2.4 m;
- estimated air volume: at least 192 m³ (80 m² × 2.4 m);
- original function: garage;
- later function: thermally insulated kitchen, dining room and family community space.

Several people regularly spent time in the room. During one trial, the temperature rose so high that those present asked for the system to be shut down.

### 8.3 Pipe network

The heating network was an extensive system serving several parts of the buildings. The exact pipe length is not documented. Based on recollection, an order of magnitude of at least 100 metres certainly existed, and the total length may have been considerably greater. The previously mentioned estimate of 450 metres cannot be verified, but given the large complex it cannot be ruled out.

The correct description is: *"a combined pipe network of at least one hundred metres, probably several hundred metres"*.

### 8.4 Buffer tank

A buffer tank with a volume of about 1 m³, i.e. 1000 litres, was connected to the system. The buffer tank:

- was permanently in the main water circuit;
- was not bypassed in normal operation;
- provided considerable thermal inertia;
- reduced sudden temperature fluctuations;
- allowed continuous engine operation under varying heat demand.

### 8.5 Circulation

Two circulation pumps were used: the pump of the engine–heat exchanger circuit and the pump of the building's radiator circuit. Pump speeds and flow conditions were adjusted experimentally. The aim was that:

- the engine temperature should remain stable;
- the heat exchanger should operate with an adequate temperature difference;
- there should be sufficient mass flow in the radiator circuit;
- neither excessively rapid local boiling nor insufficient heat removal should occur;
- adequate energy transfer should take place between the buffer tank and the building circuit.

### 8.6 Pressure conditions

The heating system operated as a closed (sealed) system. Typical pressure: sustained above 2 bar, approaching 3 bar at high thermal load. The exact time profile of the pressure and the full configuration of the safety fittings cannot be documented retrospectively.

The pressure of nearly 3 bar shows that under high thermal load the system approached the upper operating range of conventional closed heating systems.

## 9. Thermal energy calculations

### 9.1 Fuel energy per hour

```
E_1h = 3 m³ × 34 MJ/m³ = 102 MJ  ≈ 28.33 kWh
```

Thus approximately 28.3 kWh of fuel energy entered the system in one hour.

### 9.2 Theoretical heating of the 1000-litre buffer

The specific heat capacity of water is c_p ≈ 4.184 kJ/(kg·K), the water mass of the buffer tank is m ≈ 1000 kg, and the initial water temperature according to recollection was T₀ ≈ 16–18 °C (17 °C in the calculation).

If all the energy input heated only the 1000 litres of water, with no losses and no other heat-storing mass, then in one hour:

```
ΔT = 102 000 kJ / (1000 kg × 4.184 kJ/kgK) ≈ 24.4 °C
T₁ ≈ 17 + 24.4 ≈ 41.4 °C
```

This is only an idealised calculation. In reality the energy went simultaneously into the buffer tank, the radiators, the pipes, the room air, the building structure, the metal of the engine and the heat exchanger, and partly into the surroundings.

### 9.3 Theoretical heat-up times

Theoretical time to heat 1000 litres of water from 17 °C, without losses, at a power of 28.33 kW:

| Target temperature | ΔT | Energy required | Theoretical time |
|---|---|---|---|
| 40 °C | 23 K | ≈ 26.73 kWh | ≈ 0.94 h |
| 50 °C | 33 K | ≈ 38.35 kWh | ≈ 1.35 h |
| 60 °C | 43 K | ≈ 49.98 kWh | ≈ 1.76 h |
| 70 °C | 53 K | ≈ 61.60 kWh | ≈ 2.17 h |
| 80 °C | 63 K | ≈ 73.22 kWh | ≈ 2.58 h |

These figures do not mean that the radiators could only heat up after the overall average buffer temperature had been reached. The flow-line temperature could have been higher than the buffer average, immediate perfect mixing did not necessarily occur, the inlet sections of the radiators could receive high-temperature water directly, and the local surface temperature could significantly exceed the average temperature of the whole water volume.

Therefore the observation that some radiators became extremely hot within just over an hour does not contradict the energy balance.

### 9.4 Heating load of the 450 m² complex

The exact heat loss of the whole building cannot be reconstructed, because the wall construction, insulation level and windows/doors of every part of the building, as well as the outdoor temperature, the air exchange and the internal heat gains, are not known.

The fuel input of 28–30 kW related to 450 m²: 28 300 W / 450 m² ≈ **62.9 W/m²**.

This specific input power may have been sufficient for background heating of a moderately insulated large building complex, for heating the workshop and warehouse, and for rapidly overheating a well-insulated community room — especially if not all spaces were heated to the same internal temperature.

The full 28.3 kW obviously cannot be attributed to the 80 m² kitchen–dining room alone, because the system heated several spaces at the same time. It is likely, however, that high radiator output and a high flow temperature were available in that room.

## 9/A. Thermal inertia of the complete system and cyclic heat maintenance

### 9/A.1 Purpose of this supplement

For a correct assessment of the prototype's operation, the following must be distinguished: the initial heat-up of the cold or partly cooled system; the warming-through of the whole water circuit, the radiators and the building structure; the subsequent heat-maintenance operation; and the short, cyclic reheating runs of the engine.

The earlier energy calculations on their own showed only how much energy can theoretically be introduced into the system by burning a given quantity of natural gas. They did not adequately show that the prototype did not operate as a continuous, constant-output boiler. In real operation, after a longer initial heat-up, the engine was started only intermittently. A significant part of the heat supply was provided, while the engine was stopped, by the previously heated system with its large thermal mass.

This supplement does not alter the law of conservation of energy, and it does not claim that the heat-storing mass produced energy by itself. It explains how the large heat storage capacity made possible:

- operation of the engine at a favourable, stable operating point;
- avoidance of continuous part-load operation;
- less frequent and shorter reheating cycles;
- slow cooling of the entire building complex;
- a time-averaged consumption much lower than the instantaneous gas consumption of 3 m³/h.

### 9/A.2 Main components of the thermal mass

The heat storage capacity of the system was not provided solely by the 1 m³ buffer tank. The total thermal mass included: about 1000 litres of water in the buffer tank; the water content of the pipe network of at least one hundred, probably several hundred metres; the water in the radiators; the metal of the buffer tank, pipes and radiators; the mass of the engine block and the heat exchanger; the floors, walls and fittings of the workshop, warehouse and community room; and the total warmed-through structural mass of the approximately 450 m² building complex.

The exact total water volume and structural heat capacity are not documented, so the overall heat storage cannot be calculated as a single exact value. The 1000-litre buffer on its own, however, is suitable for a lower-bound estimate of the thermal inertia of the system.

### 9/A.3 Heat storage of the 1000-litre buffer tank

```
Q = m × c_p × ΔT
Q_1K = 1000 × 4.184 / 3600 ≈ 1.162 kWh  (per 1 °C change)
```

| Temperature difference | Stored heat |
|---|---|
| 5 °C | ≈ 5.81 kWh |
| 10 °C | ≈ 11.62 kWh |
| 20 °C | ≈ 23.24 kWh |
| 30 °C | ≈ 34.86 kWh |
| 40 °C | ≈ 46.48 kWh |

For example, if the average buffer temperature fell from 80 °C to 60 °C, the water mass of the buffer alone released about 83 680 kJ ≈ 23.24 kWh of heat. To this was added the energy stored in the pipe network, radiators, metal components and building structure.

### 9/A.4 Estimated additional capacity of the complete water circuit

The exact quantity of water outside the buffer is not known. As an illustrative estimate, over a 20 °C temperature difference: an additional 100 litres of water stores ≈ 2.32 kWh, 200 litres ≈ 4.65 kWh, 300 litres ≈ 6.97 kWh, and 500 litres ≈ 11.62 kWh of energy.

If the pipe and radiator circuit outside the buffer tank contained, for example, 200–400 litres of water, then over a usable temperature range of 20 °C the heat storage of the whole water circuit would be approximately 27.89 kWh for 1200 litres, 30.21 kWh for 1300 litres and 32.53 kWh for 1400 litres. This is only an illustrative range; in the absence of the actual water volume it cannot be treated as measured data.

### 9/A.5 Heat storage effect of the building structure

The heated building did not represent a heat load consisting only of air. During the heat-up phase, energy was absorbed by the walls, the concrete floor, the ceiling slab, the machinery and stored goods, the furniture, and the metal of the radiators and pipework. The heat capacity of the room air is relatively small in comparison.

Heating the approximately 192 m³ of air in the community room (≈ 230 kg, c ≈ 1.0 kJ/(kg·K)) by 10 °C requires only about 2300 kJ ≈ 0.64 kWh. The air itself can therefore be heated quickly. The slow cooling of the system was caused not by the air but primarily by the large physical mass of the water, the radiators, the pipework, the building structures and the complex as a whole.

### 9/A.6 Difference between heat-up energy and heat-maintenance energy

During a cold-start heat-up, it was necessary not only to make up the instantaneous heat loss of the building, but also to put energy into the cold water circuit, the buffer tank, the radiators, the pipes, the material of the engine and the heat exchanger, and the cooled-down structures of the building.

In the heat-maintenance phase, however, the system was already charged with thermal energy. At that point the engine's main task was only to make up the instantaneous heat loss of the building, to compensate for the slow temperature drop of the buffer, and to restore the desired flow temperature of the radiator circuit. Therefore the power and running time required for heat-up cannot be compared directly with the later heat-maintenance consumption.

### 9/A.7 Cyclic operation of the engine

The engine speed could not be reliably reduced below 350 rpm, because combustion could become more irregular, the stabilising effect of the flywheel decreased, the risk of stalling increased, the load of the generator and the mechanical drive became proportionally larger, and the uniformity of lubrication and gas exchange could deteriorate.

The system therefore could not reduce its heat output steplessly to a very low level, as a modern modulating boiler does. Cyclic operation became the practical method of control:

1. start the engine;
2. run in the stable range of 400–410 rpm;
3. reheat the buffer and the flow water;
4. stop the engine;
5. release heat from the buffer and the whole system;
6. restart when the temperature drops.

The engine thus ran for short periods at high, stable output and then stood idle for longer periods.

### 9/A.8 Time-averaged gas consumption

The measured natural gas consumption of the engine while running was about 3 m³/h. The average consumption during the heat-maintenance period, however, was determined by the actual running time per hour:

```
V̇_avg = V̇_run × t_r     (t_r = fraction of running time within one hour)
```

| Running time per hour | t_r | Average gas consumption | Average fuel power |
|---|---|---|---|
| 5 min | 0.083 | ≈ 0.25 m³/h | ≈ 2.36 kW |
| 10 min | 0.167 | ≈ 0.50 m³/h | ≈ 4.72 kW |
| 15 min | 0.25 | ≈ 0.75 m³/h | ≈ 7.08 kW |
| 20 min | 0.333 | ≈ 1.00 m³/h | ≈ 9.44 kW |
| 30 min | 0.50 | ≈ 1.50 m³/h | ≈ 14.17 kW |

According to recollection, there were times when the engine only had to be started for a few minutes or about ten minutes per hour. On this basis, during the heat-maintenance phase of the already warmed-through system, the hourly average gas consumption may at times have been in the range of approximately 0.25–0.50 m³/h; over 24 hours this corresponds to 6–12 m³/day.

These are exclusively examples calculated from the given cycle times. They cannot be regarded as documented consumption data for a full winter season, because the running time depended on the outdoor temperature, the current use of the heated areas, the state of the radiator valves, the pump settings and the switching temperatures of the buffer.

This explains how, with an instantaneous engine input power of about 28 kW, the longer-term average heat demand of the whole building complex could be substantially lower. During its short running periods the engine charged the thermal store at high heat output, and the stored energy was then delivered to the building over a longer period.

### 9/A.9 Downtime that can be covered from heat storage

Considering only the 1000-litre buffer, with a usable temperature difference of 20 °C (Q ≈ 23.24 kWh), the theoretical heat supply time is:

| Average heat demand | Theoretical time |
|---|---|
| 4 kW | ≈ 5.81 h |
| 6 kW | ≈ 3.87 h |
| 8 kW | ≈ 2.91 h |
| 10 kW | ≈ 2.32 h |
| 15 kW | ≈ 1.55 h |

In the actual system, the radiators, pipes and building structures stored additional energy, so a perceptible cooling of the rooms may have occurred over a longer period than this. The calculation also confirms that reheating for a few minutes per hour may have been physically possible, provided that the instantaneous heat loss of the building was lower, the buffer operated over a wider temperature range, the structural mass was already warmed through, and the weather did not represent the maximum winter load.

### 9/A.10 Why could the system not cool down quickly?

The continuously running circulation pumps did not prevent the system from eventually losing all its energy, but they distributed the stored heat more evenly: the temperature difference between the buffer and the radiator circuit decreased, hot water continued to reach the distant radiators, the entire water mass took part in releasing heat together, and rapid local cooling was reduced.

The pump did not produce heat, and circulation on its own did not improve the thermodynamic efficiency. It did, however, distribute the available thermal energy better and delayed the rapid cooling of individual distant sections or sections with a small water volume.

### 9/A.11 Role of the high flow temperature

One observed characteristic of the system was the extremely high radiator and flow temperature. As a result, the specific heat output of the radiators increased significantly, the rooms heated up quickly, and engine operation at 400–410 rpm represented too much heat output relative to the instantaneous heat demand — the system therefore required cyclic control.

A high flow temperature does not in itself prove a higher fuel efficiency. It demonstrates that the system was able to deliver high heat output in concentrated form to the heating circuit. The engineering basis for good overall energy utilisation was the combination of the following elements: recovery of engine cooling heat, recovery of exhaust heat, large heat exchanger surface, stable operating point, limited electrical co-generation, large thermal storage capacity, cyclic operation.

### 9/A.12 Divergence between the engine-side and the building-side optimum

- **Engine-side optimum:** the stable and favourable operating point of the machine (400–410 rpm, stable combustion, low noise, smooth running, easily controllable cooling).
- **Building-side optimum:** the instantaneous heat output that just covered the heat loss of the building — this was lower.

The difference between the two optima was bridged by the buffer tank and the thermal mass. The engine ran for short periods at its own optimum operating point, and the building received the required average power from the heat store over a longer period.

**This is one of the most important operating principles of the system.**

### 9/A.13 Required heat-absorption capacity

The prototype quickly overheated the available heating network, and in particular the community room. This indicates that the engine's minimum stable heat output exceeded the continuous heat-absorption capacity available at the time. Continuous operation would have required a larger heated area, a larger buffer store, more building sections with continuous heat demand, a polytunnel or greenhouse, domestic hot water production, or process heat use.

The defensible engineering statement:

> "The minimum stable heat output of the prototype exceeded the instantaneous heat demand of the community room in question several times over. Continuous operation of the unit would have required a substantially larger constant heat-absorption capacity."

### 9/A.14 Relationship between heat storage and efficiency

Large thermal inertia on its own does not increase the amount of energy that can be extracted from the fuel. A heat storage system can, however, improve practical, seasonal operation, because it reduces unstable part-load periods, allows operation at the optimum engine speed, reduces excessively frequent starts, moderates temperature fluctuations, and decouples heat production from heat use in time.

Therefore two separate indicators must be used when assessing the prototype: the **instantaneous overall efficiency** and the **periodic or seasonal gas consumption**. In the absence of measurement data for these, the short heat-maintenance cycles indicate good practical operation but do not prove an exact seasonal efficiency.

### 9/A.15 Corrected engineering conclusion

It is not correct to assess the operation of the prototype solely on the basis of the first heat-up from a cold state. The essential operation of the system: the gas engine produced considerable heat output in a short time at a stable operating point; the heat entered the heating system; the buffer, the water network, the radiators and the building structure stored a large amount of energy; heating continued for a longer period after the engine was stopped; and at times maintaining the temperature required only a few minutes, or about ten minutes, of engine operation per hour.

This mode of operation does not prove a thermodynamic efficiency several times higher, but it confirms the practical viability of a cyclic system based on large thermal storage. For continuous operation of the prototype, a larger heat-absorbing side — for example a larger property, or a workshop, warehouse or polytunnel system — would have been more suitable.

## 10. Observed natural validation phenomena

### 10.1 Room overheating

During one operating trial, the temperature of the community room of more than 80 m² rose to a level that was hard for people to bear, and the occupants asked for the system to be shut down. This is not a numerical temperature measurement, but it is strong qualitative evidence that the radiator circuit delivered high heat output within a short time.

### 10.2 Injury from touching a radiator

When the radiator surface was checked by hand, touching it caused a burn, or at least an immediate, severe thermal injury. No exact radiator temperature can be derived from this, but the observation confirms that the radiator surface was not simply warm but dangerously hot.

### 10.3 Paint damage on new radiators

The heating system had been refurbished immediately before the experimental period, and the radiators were newly installed. Under high thermal load, the paint cracked around the inlet connections, flaked off in places, and the radiator panel became locally deformed or bulged.

Paint damage on its own is not suitable for determining an exact water temperature, but together with the other observations it is significant empirical evidence. The statement in the earlier study of "a water temperature of at least 95 °C" was therefore an overly precise claim. The correct finding:

> "An extremely high local temperature, not documented by instruments, and thermo-mechanical stress developed at the inlet section of the radiators."

### 10.4 Low noise

The engine operated in an open space, without a separate acoustic enclosure, and its operation was extremely quiet. This is not a standardised decibel measurement.

The quiet operation was probably due to a combination of the extremely low speed of about 400 rpm, the four-cylinder design, the large flywheel mass, the uniform mechanical load, the stable gas operation and the absence of higher-frequency combustion and mechanical noise.

## 11. Electricity generation

### 11.1 Verified load

At times, a power of about 1 kW was drawn from the 48-volt battery system. At 48 V this corresponds to a current of I = 1000 W / 48 V ≈ 20.8 A — an order of magnitude that is realistic for the generator, the rectifier and the battery system.

### 11.2 The 2 kW estimate

The earlier study assumed an electrical output of about 2 kW. At 48 V this would require ≈ 41.7 A. This is a mechanically possible current for a 48-volt generator from a forklift, but there is no certified measurement record confirming a continuous output of 41–42 amperes. The correct classification is therefore:

- verifiably handled load: about 1 kW, intermittently;
- probable electrical output range: about 1–2 kW;
- 2 kW: upper estimate, not a laboratory measurement result.

### 11.3 Electrical efficiency

At 1 kW output, η_el ≈ 1 / 28.33 ≈ 3.5%; at 2 kW output, η_el ≈ 7.1%. Both values are low compared with conventional power-generating gas engines; this is, however, consistent with the purpose of the system: the mechanical and electrical output was deliberately treated as secondary to heat production.

## 12. Estimated heat output and overall efficiency

### 12.1 What can be calculated with certainty?

Known with certainty or to a good approximation: the fuel input of about 28.3 kW; the verified intermittent electrical output of about 1 kW (estimated at no more than about 2 kW); that the system utilised both cooling-circuit and exhaust-side heat; that the engine and the heating system operated on a sustained basis; and that a significant quantity of heat reached the radiator circuit.

Not known: the flow and return water temperatures, the actual water mass flow, the exhaust gas mass flow, the gas inlet and outlet temperatures of the heat exchanger, the losses to the surroundings, and the exact efficiency of the generator and the DC–DC converter. Therefore the useful heat output cannot be determined as a single exact number.

### 12.2 Conservative energy balance

```
P_in = P_el + Q_useful + P_loss
```

| Total utilisation | Useful electricity + heat | Estimated useful heat (with 1–2 kW electrical) |
|---|---|---|
| 70% | ≈ 19.83 kW | ≈ 17.8–18.8 kW |
| 80% | ≈ 22.66 kW | ≈ 20.7–21.7 kW |
| 85% | ≈ 24.08 kW | ≈ 22.1–23.1 kW |
| 90% | ≈ 25.50 kW | ≈ 23.5–24.5 kW |

In conventional CHP systems, total utilisation is often in the range of around 60–80%. The present prototype was a different system, specifically tuned for heat production; because of the large-surface heat exchanger, the full integration of engine cooling and the non-public proprietary design solution, higher utilisation is possible in principle. The value of 95.3%, however, cannot be proven retrospectively.

### 12.3 Assessment of the earlier 25 kW heat estimate

If P_in = 28.33 kW, P_el = 2 kW and Q_heat = 25 kW, then η_total = (2 + 25) / 28.33 ≈ 95.3%. This is mathematically correct, but its engineering status is: not a measured result, not a proven actual efficiency, but an upper-bound estimation scenario. The correct statement of the study:

> "The useful heat output of the prototype was probably in the range of 18–24 kW. The earlier value of 25 kW is a possible upper estimate, which would correspond to an overall energy utilisation of about 95%. This has not been directly confirmed by instruments."

### 12.4 What nevertheless supports high utilisation?

High heat utilisation is supported by the following combination of circumstances: the extremely low mechanical efficiency of the engine; full integration of engine cooling heat into the heating; recovery of exhaust heat; a significantly oversized heat exchanger; low gas-side throttling; a consistently stable engine temperature; a large heated complex; a 1000-litre buffer; extremely hot radiators; room overheating; and two full winter seasons of real operation. These do not replace calorimetric measurement, but they constitute strong empirical validation.

## 13. Operating time and durability

The prototype was used over two winter seasons. The first heating period lasted approximately from the end of October to March; operation was repeated the following winter. Individual runs included continuous operation of a few hours, several hours and several tens of hours. The system was not a one-off demonstration or a trial lasting a few minutes.

The system was eventually dismantled for reasons other than technical failure. At that time there was no external interest in further development and exploitation.

## 14. Technical classification

| Category | Content |
|---|---|
| **Measured** | approx. 3 m³/h natural gas consumption with a certified gas meter; 400–410 rpm with a laser tachometer; 48-volt electrical system; heating system pressure above 2 bar, rising to nearly 3 bar |
| **Observed** | operation over two winter seasons; continuous operation lasting from a few hours to several tens of hours; stable engine temperature; extremely low noise; exhaust manifold glowing red above 500 rpm; partly melted heat exchanger connection; dangerously hot radiators; cracking and flaking of radiator paint; local deformation of radiator panels; significant overheating of the community room |
| **Calculable retrospectively** | approx. 28.3 kW fuel input; approx. 102 MJ of energy input per hour; approx. 20.8 A at 1 kW, approx. 41.7 A at 2 kW; theoretical, loss-free heating of 1000 litres of water by 24.4 °C in one hour |
| **Estimated** | approx. 1–2 kW electrical output; approx. 18–24 kW useful heat output; approx. 70–90% total utilisation; pipe network of at least 100 metres, presumably several hundred metres |
| **Not verifiable retrospectively** | exact total efficiency of 95.3%; exact radiator water temperature; exact exhaust gas temperature; total instantaneous water mass flow; actual heat transfer rate of the heat exchanger; continuous 2 kW net output of the generator |

### Final technical conclusion

Based on the available data, the operation of the prototype is thermodynamically possible, mechanically consistent, empirically confirmed, validated over several months of operation and realistic from an energy standpoint. The correct classification of the unit:

> "An experimental gas-engine combined heat and power prototype, built in a workshop through functional reuse, running at extremely low speed and optimised for heat production."

The system cannot be regarded as a fully instrumented laboratory specimen, but neither is it a mere theoretical concept. It was a physically built unit that was operated repeatedly and performed an actual heating duty over two winter seasons.

## 15. Possibility of reconstruction

The system could be rebuilt with present-day equipment. A modern reconstruction would require the following measurement system: certified gas volume measurement; gas pressure and temperature measurement; flow and return water temperatures; volumetric flow in the engine cooling circuit and the radiator circuit; exhaust gas inlet and outlet temperatures; exhaust-side pressure drop; flue gas O₂, CO₂, CO, NOₓ and hydrocarbon content; engine speed; shaft torque; generator voltage and current; input and output power of the DC–DC converter; stratification temperatures of the buffer tank at several heights; and an estimate of heat loss to the surroundings.

```
Q̇ = ṁ × c_p × (T_flow − T_return)
η_total = (P_el,net + Q̇_useful) / P_fuel
```

With this, the prototype of the time could today be turned into a precisely measurable and reproducible engineering system.

## 16. Intellectual value and the limits of disclosure

The value of the prototype did not lie merely in connecting an old gas engine to a heat exchanger. The main value is represented by the non-public proprietary technical solution that determined the stable combustion at extremely low speed, the ratio between heat production and mechanical output, the control of the engine's operating temperature, the efficient extraction of exhaust-side heat, the interaction of the heat exchanger and the two liquid circuits, and the overall operating optimum of the system.

This document records the existence and function of this solution, but does not disclose its exact design. The purpose of the public part is the historical documentation of the prototype, the engineering verification of its functionality, the demonstration that the energy balance is realistic, and the presentation of the development principle. The non-public part contains the know-how without which similar efficiency and stable operation of the system are not necessarily reproducible.

## 17. Later offline AI integration

The offline AI system is not part of the proven operation of the original experiment; it is a development direction added later. In principle, the gas-engine energy centre could be suitable for continuous baseload electricity generation, for charging battery energy storage, for supplying heat and electricity to local server infrastructure, and for further use of the servers' waste heat for space heating.

A large, multi-GPU offline AI cluster, however, cannot be supplied directly at full load from the original 1–2 kW generator output. A large cluster must be treated as a separate energy subsystem (high-capacity battery buffer, several parallel energy sources, inverter-based and DC-bus power distribution, intermittent high-power runs, with the gas-engine unit as a partial charging and heat-generating module). Its detailed design is the subject of a separate engineering study and must not be confused with the measured results of the original prototype.

## Summary

The basic idea of the experimental system was to treat the limited mechanical efficiency of a conventional Otto engine not as a disadvantage but as an opportunity for heat production. The solution:

- saved a working engine and generator from destruction;
- gave the subassemblies of the donor unit a new function;
- created a stable heat source through low-speed gas operation;
- utilised both engine cooling heat and exhaust heat;
- contributed to heating a complex of about 450 m²;
- provided electrical co-generation;
- operated for two full winter seasons.

The input power of about 28.3 kW calculated from the natural gas consumption of 3 m³/h is consistent with the high heat production observed. The probable useful heat output can conservatively be placed in the range of about 18–24 kW; the electrical output was probably about 1–2 kW. The previously stated heat output of 25 kW and overall efficiency of 95.3% cannot be ruled out with complete certainty, but in the absence of direct measurement data they cannot be treated as verified results.

The real engineering value of the prototype is the combination of three elements:

1. functional industrial reuse;
2. unusual engine operation optimised for heat production;
3. the non-public proprietary design solution that made the favourable thermal operation and stability possible.

**The system could have worked in the form described, and — based on several months of actual operation over two winter seasons — it did.**
