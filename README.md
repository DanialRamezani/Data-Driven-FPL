# Data-Driven-FPL
This repo includes code for the paper "A data-driven framework for team selection in Fantasy Premier League"

The study introduces a deterministic and robust optimization framework for Fantasy Premier League (FPL) team selection. It integrates predictive modeling and integer programming to maximize expected points under FPL’s operational constraints—budget, formation, and club quota (maximum of three players per team).

The framework produces transparent, reproducible recommendations for the starting XI, captain, and bench, with extensions for robust and hybrid decision-making.

**Key Contributions**

- Optimization-Based Lineup Selection:
Mixed-integer linear programming (MILP) models that select the starting XI, bench, and captain simultaneously under FPL rules.

- Hybrid Predictive Metric:
Combines realized FPL points with forecasts from a ridge regression model trained on interpretable features such as ICT index, expected goals (xG), expected assists (xA), expected goal involvements (xGI), and starts.

- **Forecasting Approaches:**
Comparative evaluation of multiple estimation methods for expected points, including:

   -Simple and weighted averages

- Exponential smoothing

- ARIMA (Auto-Regressive Integrated Moving Average)

- Monte Carlo and bootstrap simulations

- Linear trend and hybrid ridge regression models

- Robust Optimization:
A worst-case decision model to hedge against overestimation errors in expected scores.

Empirical Evaluation:
Out-of-sample tests on the 2023/24 Premier League season reveal that ARIMA with a rolling window and recency-weighted averages perform most consistently.
