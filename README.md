# Reinforcement Learning Grid Navigation Agent
This project implements a reinforcement learning agent to navigate a grid world with obstacles and a reward location. The agent learns through Q-learning to find the shortest path to the reward while avoiding obstacles.

## Definitions:

- **Environment**: A grid world with rows and columns.
- **States**: Each cell in the grid represents a state.
- **Actions**: Up, down, left, right movement options.
- **Rewards**: Rewards are assigned to certain states (positive for the goal, negative for obstacles, -1 for other states).
- **Q-values**: A 3D array storing the expected future reward for taking each action in each state.
- **Epsilon**: Probability of choosing the best action (exploitation) vs. a random action (exploration).
- **Discount factor**: Weight given to future rewards compared to immediate rewards.
- **Learning rate**: How quickly the agent updates its Q-values based on experience.
- 
## Components:

- q_values: Stores Q-values for each state-action pair.
- rewards: Reward assigned to each state.
- is_terminal_state: Checks if a state is the goal location.
- get_starting_location: Randomly chooses a non-terminal starting point.
- get_next_action: Chooses the next action based on epsilon and Q-values.
- get_next_location: Updates the agent's location based on chosen action.
- get_shortest_path: Uses learned Q-values to find the shortest path to the goal from any starting point.
- 
## Training:

The agent interacts with the environment, exploring and updating its Q-values through Q-learning.

## Output:

Trained Q-values representing the agent's knowledge of the environment.

Shortest paths to the goal from different starting points.
