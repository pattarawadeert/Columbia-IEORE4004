**Columbia-IEORE4004: OPTIMIZATION MODELS AND METHODS**
Spring 2024 Class At Columbia University - OPTIMIZATION MODELS AND METHODS	

**Portfolio Optimization with Gurobi**

This project tackles a constrained mean-variance portfolio optimization problem, utilizing the Gurobi optimizer to handle both long and short positions while satisfying structural constraints. The project also simulates and evaluates portfolio performance over time based on asset price variations.

**Project Description**

The primary objective is to build an optimized investment portfolio by:

1. Extracting and cleaning data from the w5000.csv dataset to compute a vector of average returns and a covariance matrix.
2. Solving the optimization problem using Gurobi with constraints, such as:
- Minimum and maximum asset positions.
- Constraints on long and short positions.
- Binary conditions to ensure asset inclusion or exclusion.
3. Simulating portfolio performance over 100 days with random fluctuations in asset prices to observe the impact on portfolio value.

The methodology ensures adherence to real-world constraints and provides meaningful insights through simulation and visualization.

**Key Features**

- Data Preprocessing:
        - Cleaning assets with missing or extreme data.
        - Generating a subset of usable assets exceeding 1,800 stocks.
- Optimization:
        - Risk minimization using variance and return trade-offs.
        - Flexibility in tuning parameters like risk aversion and asset limits.
- Simulation:
        - Randomized day-to-day asset price adjustments.
        - Portfolio evolution visualization with an initial value of $1 billion.

**Implementation Overview**

- Data Preprocessing
        - Handle missing data and outliers.
        - Exclude assets with high volatility.
- Optimization
        - Objective function: Minimize portfolio risk adjusted by a risk aversion factor.
        - Constraints:
                - Position limits for individual assets.
                - Binary constraints for long and short sides.
                - Portfolio balance constraints.
- Simulation
        - Simulate daily price changes using asset-specific returns and standard deviations.
        - Adjust portfolio value dynamically and visualize performance.
- Requirements
        - Python
        - Gurobi Optimizer
        - NumPy, Pandas, Matplotlib

**How to Run**
1. Clone this repository.
2. Install the dependencies using:

pip install -r requirements.txt

3. Run the Jupyter Notebook Project6_Portfolio_Optimization.ipynb to reproduce results.

**Outputs**
- Optimized portfolio composition for different risk aversion levels.
- Simulation of portfolio performance over 100 days.
- Visualizations of portfolio value changes.

**Contribution**
Feel free to submit pull requests or raise issues for improvements.
