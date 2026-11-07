# chl-golf-optimization
for CHL.xlsx &amp; CHL Golf Case Study


#  CHL Golf Resort 2019: Operations Research & Decision Model

An advanced linear programming and optimization case study evaluating financial feasibility, land constraints, and golfer enjoyment indices for Cunningham Holdings Limited (CHL).

-----------------------------------------------------------------------------------------------

##  Project Overview
This repository contains the quantitative decision models, constraints analysis, and Solver implementations for constructing the international-standard **Cunningham Gudgal Golf Resort** at Charters Towers. 

Using Microsoft Excel and Solver, this project translates complex management and shareholder requirements into mathematical decision models to maximize golfer enjoyment while strictly adhering to capital budgets and land limits.

------------------------------------------------------------------------------------------------

##  Repository Contents
* **`CNL.xlsx`**: The primary Excel workbook containing the 5 decision models, Solver configurations, parametric data, and Answer/Feasibility reports.
* **`Case study - CHL Golf 2019.pdf`**: The official case study prompt outlining background info, UN Sustainable Development goals, structural constraints, and executive directives.

-------------------------------------------------------------------------------------------------

##  Summary of Decision Models Modeled in `CNL.xlsx`

| Model | Description | Land Used (Max 42 ha) | Total Cost (Max $20M) | Enjoyment Index | Feasibility Status |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **1. Management Plan** | Standard Clubhouse (2 ha, $3.5M cost) | 40.5 ha | $19,100,000 | 32.00 | **Feasible** |
| **2. Shareholder's Request** | Exclusive Clubhouse (4 ha, $6.0M cost, +4 bonus) | 42.5 ha | $17,520,000 | 36.00 | **Infeasible** (Violates land cap) |
| **3. Option 1** | Reduced Clubhouse Size (3 ha, exclusive features) | 42.0 ha | $18,755,334 | 36.00 | **Feasible** |
| **4. Option 2** | Scaled Clubhouse Financials / Cost Adjustments | 42.5 ha | $18,755,334 | 36.00 | *Requires constraint check* |
| **5. Option 3** | Hypothetical Budget Expansion ($21.6M ceiling) | 42.5 ha | $21,600,000 | 36.00 | **Feasible** (Budget relaxed) |

---------------------------------------------------------------------------------------------------

##  Mathematical Formulation Snapshot

### **Decision Variables (X_i)**
* X_1: Straight Par 5 holes
* X_2: Dogleg Par 5 holes
* X_3: Straight Par 4 holes
* X_4: Dogleg Par 4 holes
* X_5: Long Par 3 holes
* X_6: Short Par 3 holes

### **Objective Function**
Maximize Total Golfer Enjoyment (Z):
Z = 2.0X_1 + 1.5X_2 + 1.5X_3 + 2.0X_4 + 1.75X_5 + 2.25X_6 + {Clubhouse Bonus}

### **Key Constraints**
* **Total Holes:** sum X_i = 18
* **Total Par:** 70 <={Par Sum} <= 72
* **Land Limit:** {Total Acreage} <= 42 <={ hectares}$
* **Budget Cap:** {Total Cost} <= $20,000,000 (Standard)

----------------------------------------------------------------------------------------------------

##  Key Recommendation
While the **Shareholder's Original Request** is mathematically infeasible due to the strict 42-hectare geographic boundary, **Option 1 (Reducing the exclusive clubhouse footprint to 3 hectares)** serves as the optimal recommendation. It successfully captures maximum golfer enjoyment (**36.0**) while respecting both the 42-hectare land limit and the $20M budget constraint.
