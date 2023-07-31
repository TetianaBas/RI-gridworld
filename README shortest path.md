Q-Learning Agent for Gridworld
This Python code implements a Q-learning agent to navigate a gridworld environment and find the optimal path from a random starting location to a goal location. The environment is represented as a grid, where the agent can move in four directions: up, right, down, and left.

Classes
Environment
The Environment class represents the gridworld environment. It initializes with the specified number of rows and columns. The class has the following attributes:

rows: The number of rows in the grid.
columns: The number of columns in the grid.
actions: A list of possible actions that the agent can take (up, right, down, left).
rewards: A NumPy array representing the rewards for each cell in the grid. The rewards are initialized to -100, and the goal cell is set to 100.
aisles: A dictionary mapping aisle numbers to their corresponding cell positions.
Agent
The Agent class represents the learning agent that interacts with the gridworld environment and learns using the Q-learning algorithm. The class has the following attributes:

environment: An instance of the Environment class representing the gridworld environment.
epsilon: The exploration rate, determining the percentage of time the agent explores randomly instead of choosing the best action.
discount_factor: The discount factor for future rewards in the Q-learning update equation.
learning_rate: The learning rate, controlling the speed at which the agent updates its Q-values.
q_values: A NumPy array representing the Q-values for each state-action pair in the grid.
Methods
Environment
is_terminal_state(current_row_index, current_column_index): Determines if a state (cell) is a terminal state based on its reward value.
Agent
get_starting_location(): Gets a random starting location for the agent that is not a terminal state.
get_next_action(current_row_index, current_column_index): Chooses the next action for the agent based on the epsilon-greedy strategy.
get_next_location(current_row_index, current_column_index, action_index): Computes the next location (cell) based on the current location and chosen action.
get_shortest_path(start_row_index, start_column_index): Returns the shortest path from the given starting location to the goal location using the learned Q-values.
train(episodes): Trains the agent through Q-learning by running the specified number of episodes.
