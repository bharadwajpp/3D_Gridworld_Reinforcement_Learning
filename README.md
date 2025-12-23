# 3D_Gridworld_Reinforcement_Learning
3D Gridworld Reinforcement Learning using Q-Learning. Implements a stochastic 3D navigation environment with obstacles, goal, and pits. Features tabular Q-learning, ε-greedy exploration, policy evaluation, convergence analysis, and 3D value function visualizations.
# 3D Gridworld Reinforcement Learning using Q-Learning

## Overview
This project implements a 3D Gridworld navigation problem using Markov Decision Processes (MDP) 
and tabular Q-Learning with ε-greedy exploration. The agent learns an optimal policy in a stochastic environment.

## Environment
- Grid: 6x6x6 (height x width x depth)
- Start: (0,0,0)
- Goal: (5,5,5), Pit: (2,2,2)
- Obstacles: 25 (12% of grid)
- Actions: ±x, ±y, ±z
- Transition: slip probability = 0.2
- Rewards: step = -1, goal = +50, pit = -50
- Discount factor: γ = 0.95

## Implementation
- Q-Learning with adaptive ε-decay
- Policy evaluation over 100 test episodes
- Comparison against random policy
- Experiments with γ, slip probability, and step cost
- Visualizations: value function heatmaps, policy arrows, learning curves

## Results
- Learned policy success rate: 100%
- Mean reward: -94.47 ± 98.61
- Random policy success rate: 16%
- Improvement: +112.61 reward (54.4% better than random)

## Technologies
Python, NumPy, Pandas, Matplotlib, Seaborn
