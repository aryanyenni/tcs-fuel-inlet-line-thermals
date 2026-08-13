## Thermal Control System - 01 Fuel Inlet Line Thermal Analysis

### Background

TCS: The Yellow Jacket Space Program (YJSP) is developing Elytra, a space-bound liquid KeroLOX rocket. The Thermal Control System is responsible for maintaining all vehicle components within their operational temperature ranges during ground operations.
---

### Problem Statement

The Fuel Inlet Line in the rocket's powerhead has had a problematic past due to its complex thermal environment. RP-1 fuel is susceptible to gelling at and below 240K, which can restrict or completely block propellant flow through feed lines.

Problem Statement: Keep RP-1 in the Fuel Inlet Line above its gelling threshold of 240K for a 1.5 hour ground operations window pre-launch under worse-case thermal conditions in the powerhead region.

In this low fidelity 1D sim, the dominant heat transfer mechanisms include:
- Natural convection between powerhead air and Fuel Inlet Line, LOX Inlet Line, and outer tank wall interior
- Forced external convection between the outer tank wall exterior and the freestream
- Conduction through non-moving fluids, solid lines, and insulation
---

### Repo Structure
yjsp-tcs-rp1-thermal/
│
├── README.md
├── references/
│ └── Cebeci 1974.pdf
│
├── matlab/
│ ├── getNusselt_natural.m
│ ├── getNusselt_forced_internal.m
│ ├── getNusselt_forced_external.m
│ 
│
├── simulink/
│ ├── st_transient_ODE1.slx
│ ├── st_transient.slx
| └── st_transient_parameters.m
│
└── figures/
| ├── st_steady_preTRN.png
| ├── st_transient_ODE1.png
| └── st_transient.png
---

### Assumptions / Limitations
### Results
### Path Forward
