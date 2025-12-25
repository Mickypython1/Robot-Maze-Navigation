# Robot-Maze-Navigation
# Overview
This project demonstrates how a robot agent can learn to navigate a maze using Reinforcement Learning (RL), specifically the Q-learning algorithm. The maze is represented as a 2D NumPy array where:

0 → safe paths

1 → obstacles

The agent starts at a defined position and aims to reach a goal position, learning optimal navigation strategies through trial and error.

# Features
Maze environment built with NumPy.

Implementation of Q-learning for path optimization.

Exploration vs. exploitation strategy using epsilon-greedy policy.

Reward system:

  Penalty for hitting obstacles

  Reward for reaching the goal

  Small penalty per step to encourage shortest paths

Visualization of:

  Maze layout

  Robot’s learned path

  Training rewards over episodes

# Implementation Steps
# 1. Define Maze, Start & Goal
Maze stored as a 2D NumPy array.

Start and goal positions defined.

# 2. Initialize RL Parameters
Episodes: 5000

Learning rate (α): 0.1

Discount factor (γ): 0.9

Exploration rate (ε): 0.5

# 3. Q-Learning Algorithm

# 4. Training
Agent explores maze across episodes.

Updates Q-table based on rewards and transitions.

# 5. Extract Optimal Path
Follows highest Q-values to reach the goal.

Prevents cycles using a visited set.

# 6. Visualization
Maze plotted with matplotlib.

Start and goal highlighted.

Learned path drawn clearly.

Rewards per episode plotted to show learning progress.
