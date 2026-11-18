# Optimal Planning of Agricultural Production
Linear programming model for multi-farm crop allocation under water scarcity and equity constraints in MATLAB

![Status](https://img.shields.io/badge/Status-Complete-green)
![Language](https://img.shields.io/badge/Language-MATLAB-orange)
![Application](https://img.shields.io/badge/Application-Linear_Programming-blue)
![Field](https://img.shields.io/badge/Field-Operations_Research-purple)

## ⚙️ Methodology
* **Standard-Form Formulation:** Defined 9 decision variables (`x1` to `x9`) representing acreage allocated to Sugar Beets, Cotton, and Corn across three farms, converting net return maximization into a standard minimization problem for `linprog`.
* **Resource & Quota Constraints:** Modeled physical limits for irrigable land (400, 600, and 300 acres), water availability (600, 800, and 375 acre-feet), and maximum crop quotas (600, 500, and 325 acres).
* **Land Equity Enforcement:** Added linear equality constraints ensuring each farm cultivates the exact same proportion of its total irrigable land.
* **Sensitivity & Policy Analysis:** Evaluated active constraints at the optimum, calculated the minimum return increase needed to make Corn profitable, and simulated a 40% water-reduction legislation scenario.

## 📊 Results
* **Optimal Crop Allocation:** Water availability and crop quotas acted as the primary binding constraints, prioritizing high-return Sugar Beets and Cotton while excluding Corn (`0 acres`) under baseline pricing.
* **Sensitivity Threshold:** Identified the exact percentage increase required in Corn's net return (`> £175/acre`) to enter the optimal production basis.
* **Environmental Legislation Impact:** Reducing total water usage to 60% of the baseline solution tightened the feasible region, proportionally reducing cultivated acreage and quantifying the resulting drop in total net return.
