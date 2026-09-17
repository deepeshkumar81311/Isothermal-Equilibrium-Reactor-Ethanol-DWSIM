# Isothermal Equilibrium Reactor Simulation – Ethanol Production

## Project Overview

This project models ethanol production through the gas-phase hydration of ethylene in an **isothermal equilibrium reactor** using **DWSIM**.

### Reaction

**C₂H₄(g) + H₂O(g) ⇌ C₂H₅OH(g)**

The simulation evaluates the equilibrium composition and ethylene conversion at the specified operating conditions.

## Simulation Conditions

| Parameter | Value |
|---|---:|
| Reactor | Equilibrium Reactor |
| Operating mode | Isothermal |
| Temperature | 145 °C (418.15 K) |
| Pressure | 1 bar |
| Ethylene feed | 50 mol/s |
| Water feed | 50 mol/s |
| Ethanol feed | 0 mol/s |
| Total feed | 100 mol/s |
| Reaction phase | Vapor |
| Equilibrium constant, K | 0.1443 |

## DWSIM Flowsheet

The flowsheet consists of:

**FEED → E-REACTOR → VAPOUR / LIQUID**

The equilibrium reactor is supplied with an energy stream to maintain the isothermal operating temperature.

## Results

The DWSIM result shown in the project material gives a vapor molar flow of approximately **96.8065 mol/s** with the following vapor mole fractions:

| Vapor component | Mole fraction |
|---|---:|
| Ethylene | 0.483506 |
| Water | 0.483506 |
| Ethanol | 0.0329884 |

The corresponding ethylene conversion is approximately **6.38%**, consistent with the handwritten equilibrium calculation included in the project material.

## Methodology

1. Define ethylene, water and ethanol as the simulation components.
2. Define the equilibrium reaction:
   C₂H₄ + H₂O ⇌ C₂H₅OH.
3. Set the equilibrium constant to **K = 0.1443** for the specified conditions.
4. Configure an **Equilibrium Reactor** in isothermal mode.
5. Set the reactor temperature to **145 °C** and pressure to **1 bar**.
6. Specify the feed as 50 mol/s ethylene and 50 mol/s water.
7. Solve the steady-state simulation.
8. Evaluate outlet composition and ethylene conversion.
9. Compare the DWSIM result with the equilibrium calculation.

## Repository Contents

- `simulation/` – place the final DWSIM `.dwxmz` simulation file here.
- `images/` – project screenshots and calculation evidence.
- `report/` – project report in PDF format.
- `README.md` – project documentation.

## How to Reproduce

Open the `.dwxmz` file in DWSIM, verify the component list, reaction definition and reactor operating conditions, and run the steady-state solver.

## Key Learning Outcomes

- Steady-state process simulation using DWSIM
- Equilibrium reactor modelling
- Gas-phase reaction equilibrium
- Material-balance and conversion calculations
- Comparison between hand calculations and process-simulation results


## Author
- Deepesh kumar
- 724CH1008