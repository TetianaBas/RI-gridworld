Reinfored learning gridworld algorithm basic case project 

This project implements a simple gridworld problem using Reinforcement Learning (RL) and the Q-learning algorithm. The goal of the agent (represented as a robot) is to navigate a grid and learn the best actions to maximize its rewards and avoid penalties.

Environment Setup:
The gridworld is represented as a 3x4 matrix with cells identified by (row, column) coordinates. There are three types of cells: win cell (reward = 1), lose cell (penalty = -1), and regular cells (reward = 0). The robot starts from a designated start cell.

Key Components:
1. State: This class represents the state of the environment. It maintains the current state of the robot, checks if it has reached the win/lose cell, and defines actions to move within the grid.

2. Agent: This class represents the RL agent. It uses Q-learning to learn the best actions for each state in the grid. The agent selects actions based on a balance between exploration (trying random actions) and exploitation (choosing actions with the highest expected rewards).

How the Learning Works:
The agent interacts with the environment by moving through the grid. During each interaction, it updates its knowledge of the grid based on rewards obtained from the current state. 
The Q-learning algorithm uses a reward mechanism to update the values associated with each state-action pair, leading the agent to learn the best actions to take in each situation.

Execution:
The main script creates an instance of the Agent class and runs the RL algorithm by calling the play method. The agent plays a fixed number of rounds (episodes) and learns from the rewards it receives. After the learning process is complete, the script displays the learned state values, indicating the expected rewards for each state in the grid.
