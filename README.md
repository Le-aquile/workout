### Workout - Reinforcement Learning Package with Game Environment

**Workout** is a reinforcement learning package that provides a game environment where agents can be trained. The package is designed to help reinforce learning concepts by providing a simple, interactive games to test RL algorithms like Q-learning, Deep Q Networks (DQN), and more.

#### Features:
- **RL Training Environment**: The `FallingGame` class provides an environment where agents learn by avoiding falling enemies, receiving rewards or penalties based on their actions.
- **Customizable Settings**: Adjust parameters such as the speed of the falling enemies, screen size, and maximum points to control the game’s difficulty.
- **State Representation**: The game state consists of player and enemy positions, which can be used by RL agents to learn optimal strategies.
- **Model Persistence**: The agent can save and load its trained model (e.g., Q-table) to resume training or test with pre-trained policies.
- **Action Space**: The agent can control the player’s movement with actions like "LEFT" and "RIGHT".


#### How to Use:
1. Create an RL agent (e.g., Q-learning agent) and set up the game environment with the `FallingGame` class.
2. Train the agent in the game by running it in training mode.

#### Example Usage:
```python
from workout import FallingGame
from agent import QLearningAgent  # or your preferred RL agent

# Initialize the game with an RL agent
game = FallingGame(training=True, agent=QLearningAgent())

# Run the game loop
game.run()
```
