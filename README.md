# Snake Game with Q-learning

This project implements a reinforcement learning agent based on Q-learning algorithm to play the classic Snake game. The agent learns to navigate the game environment, avoiding obstacles and collecting food to maximize its score.

# Introduction
The project aims to demonstrate the application of reinforcement learning to a simple environment—the Snake game. The agent uses Q-learning, a model-free reinforcement learning algorithm, to learn how to play the game by maximizing its cumulative reward

# How It Works
- Game Environment: The Snake game is implemented using Pygame, where the snake navigates a grid to collect food. The game ends when the snake collides with the walls or itself.
- Q-learning Agent: The agent observes the game state (snake and food positions) and takes actions (move up, down, left, right) based on a Q-table, which is updated through learning from experiences.
- Reward System: The agent receives positive rewards for collecting food and negative rewards for collisions, guiding it towards optimal behavior.

# Training the Agent
The agent is trained over multiple episodes. During each episode:

- The agent selects actions based on an epsilon-greedy policy.
- The Q-table is updated using the Bellman equation.
- The exploration rate decays over time to balance exploration and exploitation.
- Training progress and total rewards are printed for each episode.

# Evaluating the Agent
After training, the agent can be evaluated by running the game and observing its performance. The Q-table is used to select the best action for each game state, with no exploration.

