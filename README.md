# PCB-then-Discharging-or-Charging-of-3S1P-using-Mean-SoC-Method-for-Li-ion-Batteries-used-in-EV
This simulation project demonstrates Passive Cell Balancing (PCB) followed by discharging or charging of a 3S1P lithium-ion battery pack, based on the Mean State of Charge (SoC) method. The model is developed to emulate real-world energy management in Electric Vehicles (EVs)—specifically two-wheelers or small EVs that commonly use a 3-series, 1-parallel (3S1P) battery configuration.

The goal of this simulation is to show how passive balancing can equalize SoC among cells before energy is drawn (discharging) or stored (charging), using an intelligent Mean SoC-based strategy to initiate balancing actions.



⚙️ Key Concepts
🔋 3S1P Li-ion Configuration
3 cells connected in series (to increase voltage)

1 cell per series leg (no parallel branches)

Used commonly in compact EV applications


🧠 Mean SoC Balancing Logic
Calculates the average SoC of all three cells.

Cells with SoC above this average are discharged passively using resistors.

Balancing is triggered only when the SoC deviation exceeds a threshold, making it energy-efficient.


🔁 Post-Balancing Operation
After the balancing process stabilizes:

The pack can either discharge to simulate power delivery (e.g., during vehicle drive)
or

Charge to simulate energy storage (e.g., during regenerative braking or plug-in charging).


💡 Objectives of the Simulation
To ensure all cells are at approximately equal SoC before operation to:

 Avoid overcharging/overdischarging

 Extend battery life

 Improve system efficiency

To demonstrate a passive balancing technique that is simple, low-cost, and reliable.

To simulate real-world EV conditions using MATLAB/Simulink.


🛠️ Tools and Techniques
Software: MATLAB/Simulink

Balancing Type: Passive (Resistive bleeding)

Control Logic: Mean SoC threshold activation

Battery Chemistry Modeled: Generic Li-ion (customizable)


📈 What You’ll See in the Simulation
Real-time cell voltage and SoC curves

Triggering of balancing resistors when SoC > Mean SoC

System behavior under both discharging and charging conditions

Energy losses during balancing (optional for analysis)

Final SoC convergence before main operation


📦 Applications
Electric two-wheeler battery management

Educational models for BMS development

Research on SoC-based balancing strategies

Low-cost embedded BMS firmware testing


🔖 Future Improvements
Extend to nS1P or nSxP systems (e.g., 8S2P)

Add active balancing comparison

Integrate temperature-dependent balancing logic

Hardware implementation using microcontrollers
