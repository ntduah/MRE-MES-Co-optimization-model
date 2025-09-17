# MRE-MES-Co-optimization-model
Gurobi/Python code for capacity planning and dispatch of a standalone Marine Renewable Energy–supported Multi-Energy System (MRE-MES). Includes deterministic planning, varying-demand Monte Carlo, and two-stage stochastic models for electricity, heat, water, and hydrogen demand.
# MRE-MES Co-Optimization (Deterministic, Varying-Demand, Two-Stage Stochastic)

This repository accompanies the paper on planning a standalone Marine Renewable Energy–supported Multi-Energy System (MRE-MES) for coastal applications.  
The system couples wind, PV, and wave generation with a CHP gas turbine + boiler, reverse-osmosis (RO) desalination, a PEM electrolyzer, and storage (battery, thermal, hydrogen, water).  
Four energy carriers are modeled hourly: **electricity, heat, freshwater, hydrogen**.

## Models
- **deterministic.py** — single-trajectory capacity planning and dispatch.
- **varying_demand.py** — Monte Carlo operational study with **fixed capacities**; randomizes demands and resources and resolves dispatch repeatedly.
- **two_stage_stochastic.py** — two-stage planning with first-stage capacities and second-stage (scenario) operations (25 scenarios, equal probability).

> Original filenames:  
> `hybrid_microgrid_gurobi_standalone_var Deterministic.py`,  
> `hybrid_microgrid_gurobi_standalone_var Varying demand.py`,  
> `hybrid_microgrid_gurobi_standalone_var Two-stage Stochastic.py`.

