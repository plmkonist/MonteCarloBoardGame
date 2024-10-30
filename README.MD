
Monte Carlo Simulation of "The Perfect Balance" Board Game
Overview
This repository contains a Monte Carlo simulation of a board game designed to model the balance of stress and money management. The game centers around player strategies in work-life balance, where each player aims to earn enough to cover rent while managing stress levels to avoid burnout. This simulation evaluates different gameplay outcomes across various player strategies.

Game Rules and Mechanics
Players choose between working to earn money (at the cost of gaining stress) and destressing to reduce their stress levels. Each player faces the following conditions:

Work: Increases player money by a random amount within a range (job pay range) and adds stress. Stress from work may also include commute-related stress.
Destress: Reduces player stress by a random amount within a destress range.
Stress Limit: If a player’s stress level exceeds 15, they lose a portion of their earnings due to "burnout."
Simulation Parameters
The simulation explores different configurations based on:

Job Pay Range: Income range for each working day.
Destress Range: Stress reduction range for destressing activities.
Work Stress Gain: Amount of stress added per workday.
Commute Stress: Additional stress based on housing distance.
House Rent: Fixed rent cost due at the end of each month.
Strategies: Different approaches to work-life balance.
work-first: Prioritizes work, then destresses when necessary.
balanced: Alternates between work and destressing, aiming to balance earnings with manageable stress.
work-more: Prioritizes working more days, taking fewer destress days unless stress is high.
Running the Simulation
The run_simulations function runs the game simulation across different strategy and parameter combinations, tracking:

Final money and stress values for each player.
Success rates by strategy (percentage of players with non-negative money).
Average and standard deviation of outcomes.
Usage
Run the Simulation: Configure the n parameter in run_simulations(n) to control the number of runs per parameter configuration.
Plot Results: plot_histograms visualizes the distribution of money and stress for each strategy.
Sample Output
After each simulation run, statistical insights for each strategy are displayed:

Percentage of players with ≥ 0 money.
Average and standard deviation of final money.
