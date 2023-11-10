Q-Learning in Grid World

This project implements Q-learning in a grid world environment using Python and NumPy. The agent learns to navigate through the grid to reach the goal while avoiding obstacles, and the Q-learning algorithm is employed to optimize its actions.

Environment
The grid world is defined by an environment class, specifying the size, actions, rewards, and locations of obstacles (aisles). The goal of the agent is to reach a specific cell with a high reward.

Agent
The agent class initializes the Q-values and implements methods for training the agent through Q-learning. It also provides methods to determine the starting location, get the next action, and calculate the shortest path.

Parameters
epsilon: Exploration-exploitation trade-off parameter.
discount_factor: Discount factor for future rewards.
learning_rate: Learning rate for updating Q-values.

Results
The project demonstrates the Q-learning algorithm's ability to train an agent to navigate a grid world efficiently, finding the shortest path to the goal while avoiding obstacles.
