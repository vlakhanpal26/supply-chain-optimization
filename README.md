## Robust Supply Chain Optimization under Demand Uncertainty 

The goal is to design a supply chain network that performs well under uncertain demand conditions. Using Monte Carlo simulation to model demand variability and mixed-integer programming (MIP) for optimization, the project focuses on minimizing total costs like facility operations, production, and transportation while ensuring demand is met across multiple realistic scenarios.

The model also incorporates sustainability considerations by assigning carbon emission penalties to each transportation route. This adds a tunable environmental objective on top of the financial cost minimization, allowing trade offs between cost efficiency and also, cleaner logistics.

The motivation behind this project comes from real world supply chain disruptions and the need for networks that are not only cost efficient but also resilient to fluctuations in consumer demand.

---

## Project Objectives

- Develop a supply chain model that balances cost and reliability
- Incorporate demand uncertainty using Monte Carlo methods
- Identify the best combination of facility locations and routing plans under variable conditions
- Add a sustainability component by tracking and penalizing carbon emissions from transportation
---

## Tools

- Python ( for modeling and simulation)
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `pyomo` formulating the optimization model
- `GLPK` or `CBC` solver (open-source)
---

## Data Description

- **demand_scenarios.csv**: Contains 100 different demand simulations for 5 customer zones. Each row is a scenario, each column is a zone. Demand is sampled using realistic means and standard deviations.

- **facility_costs.csv**: Lists 3 candidate facilities with fixed opening costs and their maximum capacities.

- **transportation_costs.csv**: Contains unit shipping cost and estimated carbon emissions per unit shipped for every facility-to-zone pair.
