**Language:** [Magyar](02_200kWh_LiFePO4_felugyeleti_architektura.md) | [English](02_200kWh_LiFePO4_felugyeleti_architektura.en.md)

# 200 kWh LiFePO4 Energy Storage — Data Acquisition and Monitoring Architecture

**Preliminary technical design**

Author: Almási Andor · Base version: v1.4 (January 2026) · Public version

> **Publication note.** The public version contains the design principles of the system, the interface logic and the cell calculation. Specific inventory data, cost and labour-time calculations, and the market valuation are not part of the public version.

## 1. Project title and basic objective

HMI-based data acquisition and monitoring architecture for a 200 kWh LiFePO4 energy storage system — preliminary design.

## 2. Initial framework

| Aspect | Value |
|---|---|
| System voltage | approximately 400 V DC |
| Energy capacity | 200 kWh |
| Load | at least 250 A continuous |
| Objective | generating measurement evidence, condition monitoring, documentability, future marketability |
| Phase | data acquisition and design — not commissioning |

## 3. System-level partitioning and safe separation

**Basic principle:** protection, control and display do **not operate at the same level**.

## 4. Functional layers

| Layer | Elements |
|---|---|
| 4.1 Cell level | cells, temperature sensors |
| 4.2 Balancer and BMS level | active balancer modules; cell voltage, temperature, state of charge (SOC), faults |
| 4.3 Data acquisition and control level | gateway or PLC function |
| 4.4 HMI and supervision | display, logging, data export |
| 4.5 External world | SCADA, laptop, access for audit purposes |

This partitioning follows industrial practice, is auditable and is insurance-friendly.

## 5. Interface logic

### 5.1 Link between cells and balancer

- Hardware: dedicated active balancer modules.
- Communication: over a CAN bus or an RS-485 line, using the Modbus RTU protocol.
- Rationale: deterministic operation, noise immunity, industry standard.

The HMI does not intervene directly at this level.

### 5.2 Link between balancer and data acquisition unit

- Communication: over a CAN bus or an RS-485 line, using the Modbus RTU protocol.
- Tasks: measurement of cell voltages, temperature data, balancing status, faults and events.

**This is the layer where the data becomes authoritative.**

### 5.3 Link between gateway and HMI

- Communication: over an Ethernet network.
- Protocol: Modbus TCP or OPC-UA.
- Advantages: galvanic isolation capability, scalability, documentability.

### 5.4 Link between HMI and the external world

- Data export: via USB or SD storage media.
- Network access: over Ethernet, using the SFTP or HTTPS protocol.
- Purpose: evidence, measurement reports, audit material.

## 6. Role of the HMI

**Basic principle:** the HMI is neither a protection device nor a real-time balancer.

Tasks of the HMI: data acquisition, logging, visualisation, generation of technical evidence. Active balancing runs on separate hardware; the HMI only provides configuration and control. This is a legally and technically safe solution.

## 7. Advantages of the preliminary design

- modular;
- reversible (can be taken apart again);
- does not preclude later decisions;
- can be extended towards audit or CE conformity;
- not a dead end.

## 8. Cell calculation for 120 cells in series

### 8.1 Basic data of one cell

- Nominal voltage: 3.2 V
- Capacity: 100 Ah
- Energy content of one cell: 3.2 V × 100 Ah = **320 Wh**

### 8.2 Number of series cells and system voltage

- Number of cells in series: 120
- Nominal system voltage: 120 × 3.2 V = **384 V**

### 8.3 Energy content of one series string

- 120 cells × 320 Wh = 38 400 Wh = **38.4 kWh**
- Check: 384 V × 100 Ah = 38.4 kWh — the two methods give the same result.

### 8.4 Parallel strings needed to reach close to 200 kWh

200 kWh / 38.4 kWh ≈ 5.2 → counting whole strings: **5 parallel strings**.

### 8.5 Complete system in 120S5P configuration

- Voltage: 384 V
- Capacity: 5 × 100 Ah = 500 Ah
- Energy: 384 V × 500 Ah = 192 000 Wh = **192 kWh**

### 8.6 Total number of cells

120 series cells × 5 parallel strings = **600 cells**. Check: 192 000 Wh / 320 Wh = 600 cells.

### 8.7 Conclusion

With 120 cells in series, the nominal voltage of the system is 384 V. With five parallel strings, the total energy capacity is 192 kWh. In technically correct terms, this configuration can be treated as a system of approximately 200 kWh.

## 9. Professional note: why does cell matching matter?

For energy storage systems of close to 200 kWh with a nominal voltage of about 400 V, a continuous load capability of 250 A cannot be regarded as a standard market value. Battery packs with such parameters are typically available only to custom order, and even then they are rare.

The vast majority of commercially available high-capacity systems are built not from matched (graded) cells or packs, but from average-quality units that lie within manufacturing tolerances. The use of matched cells:

- improves current sharing;
- reduces the internal voltage spread;
- measurably increases the expected service life.

For the planned systems, a conservative figure of **8000 full charge–discharge cycles** can be assumed. For LiFePO4 chemistry this is not an optimistic but a realistically achievable value, especially with active balancing and controlled operation. For a 192 kWh system, this means a total energy throughput of approximately **1536 MWh** over the life cycle.
