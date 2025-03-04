# **Financial Derivatives and Risk Management Simulations**

This repository contains Python implementations of various financial models and simulations related to option pricing, hedging strategies, and portfolio management. These models use techniques such as Monte Carlo simulations, binomial trees, and stochastic processes under Geometric Brownian Motion (GBM) assumptions.

## **1. lattice_walk_simulation.py**
This script simulates a **random walk on a lattice** using a binomial process. It models stock price movements using up/down steps and examines the statistical properties of the resulting distribution. The simulation is run with different numbers of simulations (1,000, 10,000, 100,000) to analyze convergence.

- **Techniques Used:** Lattice walk simulation, probability density estimation  
- **Output:** Mean, standard deviation, and histogram comparing the empirical distribution to the expected normal distribution.


## **2. ito_integral_variance.py**
This script approximates the **Ito integral** and investigates its variance as the time step decreases. The simulation is performed using different numbers of time steps (100, 200, 400, ..., 6400), and the variance is plotted as a function of the time step.

- **Techniques Used:** Stochastic calculus, Ito integral, Brownian motion  
- **Output:** Convergence analysis of variance, graph of variance vs. time step.


## **3. binomial_option_pricing.py**
This script implements the **binomial tree method** to price European and American call and put options. It compares the computed option prices to the analytical solution from the Black-Scholes model.

- **Techniques Used:** Binomial tree, risk-neutral valuation, European vs. American option pricing  
- **Output:** Convergence of option prices with increasing binomial tree steps.


## **4. root_finding_methods_analysis.py**
This script compares **numerical root-finding methods** (Bisection, Newton’s, Secant, and Fixed Point Iteration) for solving non-linear equations. It calculates their orders of convergence and error ratios.

- **Techniques Used:** Numerical analysis, root-finding methods  
- **Output:** Tables showing convergence rates and errors for each method.


## **5. option_pricing_fixedpoint_newton.py**
This script applies **fixed-point iteration** and **Newton’s method** to solve for the implied option price in a Black-Scholes model. It compares the convergence speed of both methods.

- **Techniques Used:** Fixed-point iteration, Newton’s method, Black-Scholes pricing  
- **Output:** Tables showing the iteration process and convergence analysis.


## **6. monte_carlo_option_pricing.py**
This script prices **European put options** using a **Monte Carlo simulation** under a stochastic process. It analyzes convergence by varying the number of simulations and time step sizes.

- **Techniques Used:** Monte Carlo simulation, stochastic differential equations, lognormal stock price modeling  
- **Output:** Convergence of Monte Carlo estimates, confidence intervals for option prices.


## **7. delta_hedging_stochastic_paths.py**
This script simulates **delta hedging of European put options** using a single stochastic path. It tracks the evolution of portfolio value, cash holdings, and stock holdings over time.

- **Techniques Used:** Delta hedging, Black-Scholes Greeks, risk-neutral valuation  
- **Output:** Plots of stock price, portfolio value, and hedging errors over time.


## **8. cppi_simulation_gbm.py**
This script simulates the **Constant Proportion Portfolio Insurance (CPPI)** strategy under a **Geometric Brownian Motion (GBM)** assumption. It examines the impact of different floor levels and multipliers on portfolio returns and risk.

- **Techniques Used:** CPPI strategy, risk management, Monte Carlo simulation  
- **Output:** Tables showing portfolio statistics (mean return, standard deviation, Value-at-Risk (VaR), Conditional VaR), probability density plots.


## **9. covered_call_strategy_gbm.py**
This script simulates a **covered call strategy** under the **Geometric Brownian Motion (GBM)** assumption. It computes log returns, standard deviation, and risk measures for different strike prices.

- **Techniques Used:** Options trading, covered call strategy, Black-Scholes pricing  
- **Output:** Performance metrics for different strike prices, probability density plot.
