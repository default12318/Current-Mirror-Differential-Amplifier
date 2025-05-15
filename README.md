# Current-Mirror-Differential-Amplifier
This project implements a Current Mirror Differential Amplifier using SkyWater 130nm PDK. 

## Tools Used
- **Technology Node**: SkyWater 130nm
- **Design Software**:
  - `xschem` (for schematic)
  - `ngspice` (for simulation)
  - `Magic` (for layout)
  - `Netgen` (for LVS)
 
  - A Current Mirror Differential Amplifier (CM Diff Amp) is a foundational building block in analog integrated circuits.


### Circuit Components
- **M1, M2** – PMOS transistors forming the differential pair
- **M3, M4** – PMOS transistors forming the biasing circuit
- **M5, M6, M9, M10** – NMOS transistor acting as the current mirrors
- **M7, M8** – PMOS transistors forming the current mirror

---

### Working Principle
- **Inputs** \( V_{in+}, V_{in-} \) are applied to the **gates of M1 and M2**.
- M1 and M2 **source current from the biasing circuit (M3, M4)** and steer it based on the differential input voltage.
- **current mirror** to convert the differential current into a single-ended output.

## Schematic

## Interdigitised and Matching Layout dependent Schematic

## Schematic Simulations

## Layout

## LVS

##Conclusion
In this project, we successfully designed, simulated, and verified a **PMOS Differential Amplifier with an NMOS Current Mirror Load**. This design highlights essential analog IC principles, including differential signal amplification, current steering, and active loading.

By using PMOS transistors as the differential pair, the amplifier is optimized for handling **negative or low-voltage input signals**, while the NMOS current mirror acts as an active load to enhance gain and **common-mode rejection ratio (CMRR)**.

Key accomplishments include:
- ✅ **Schematic Design** using xschem
- ✅ **SPICE Simulations** using ngspice
- ✅ **Layout Design** using Magic VLSI layout tool
- ✅ **Design Rule Check (DRC)**: Passed
- ✅ **Layout vs. Schematic (LVS) Check**: Matched using netgen
- 📐 **Compact and symmetric layout** for performance and area efficiency

This differential amplifier is a fundamental building block for **operational amplifiers, analog filters, and signal processing circuits**. The full flow from schematic to layout verification was completed using the **SkyWater 130nm PDK**, preparing the design for integration into a full custom analog IC.

