# Statistical-market-making-simulation
Group 9

Sai Siddharth – 2025AIB1046
Aravind – 2025AIB1023
Sandesh Jadhav – 2025AIB1060
K. Abhiram – 2025AIB1035
B. Abhishek – 2025AIB1014

Simulation of user behavior in digital platforms using Markov chains with adaptive transition probabilities and endogenous feedback learning.
Statistical Market Making Simulation using Adaptive Markov Chains
Overview

This project models user behavior in large-scale digital platforms using a Markov-chain-based stochastic simulation framework. Unlike classical Markov models with fixed transition probabilities, this implementation introduces adaptive transition probabilities that evolve dynamically using endogenous feedback from user interactions.

The simulation demonstrates how individual random user actions produce stable aggregate behavior and how probability updates influence long-term system dynamics.

Problem Statement

Traditional Markov-chain models assume constant transition probabilities between states. However, real-world digital platforms are adaptive systems where user behavior influences future transitions.

This project proposes a simulation framework that incorporates:

time-varying transition probabilities
endogenous feedback learning
large-scale user interaction modeling
convergence analysis using stochastic processes
State Space Definition

The system models user movement across the following platform states:

Browse → Search → Click → Purchase → Exit

Each simulated user begins in the Browse state and transitions across states according to a probability matrix.

Methodology

The implementation follows these steps:

Define platform state space
Construct transition probability matrix
Simulate user movement using Markov transitions
Perform multi-user stochastic simulation (1000 users)
Introduce adaptive transition probability updates
Track probability evolution over time
Compare static and adaptive transition models
Demonstrate convergence using increasing user counts

Adaptive probability update rule:

P(i,j)(t+1) = P(i,j)(t) + α

where α represents learning rate.

Key Features

This implementation includes:

Discrete Markov state-space modeling
Multi-user stochastic simulation
Absorbing-state analysis (Purchase, Exit)
Adaptive transition probability learning
Transition probability evolution tracking
Static vs adaptive model comparison
Convergence verification using Law of Large Numbers
Visualization using probability evolution graphs
Results

Simulation results demonstrate that adaptive transition probabilities significantly influence long-term system behavior.

Example observations:

Static transition model produced higher purchase stability
Adaptive transition model shifted probability toward exit state
Transition probabilities evolved dynamically during simulation
Convergence observed as number of simulated users increased

These results validate the effectiveness of endogenous feedback learning.

Visualization Outputs

The project generates the following result graphs:

Static vs Adaptive Model Comparison
Probability Evolution (Click → Purchase)
Convergence Plot (Law of Large Numbers)

These visualizations demonstrate adaptive stochastic behavior.

Tools and Technologies Used

The project was implemented using:

Python
NumPy
Pandas
Matplotlib
Google Colab
Applications

This modeling framework can be applied in:

recommendation systems
e-commerce behavior modeling
digital platform analytics
financial market microstructure simulation
traffic flow modeling
decision process optimization
Project Structure

Repository contents:

Statistical-Market-Making-Simulation/

│── Statistical_Market_Making_Simulation.ipynb
│── comparison_plot.png
│── probability_evolution.png
│── convergence_plot.png
│── README.md
│── report.pdf


References
H. Markowitz, Portfolio Selection: Efficient Diversification of Investments
R. Cont and P. Tankov, Financial Modelling with Jump Processes
G. Grimmett and D. Stirzaker, Probability and Random Processes
J. R. Norris, Markov Chains
