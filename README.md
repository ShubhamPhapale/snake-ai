# Snake AI

This project implements an AI agent that learns to play the classic game of Snake using reinforcement learning techniques. The AI utilizes a Deep Q-Network (DQN) to make decisions and improve its performance over time.

## Features

- Custom Snake game environment built with Pygame
- Deep Q-Network (DQN) implementation using PyTorch
- Experience replay for efficient learning
- Epsilon-greedy exploration strategy
- Visualization of training progress

## How it works

1. The agent observes the current game state (snake position, food position, obstacles).
2. It uses the trained neural network to predict the best action (move direction).
3. The action is executed in the game environment.
4. The agent receives a reward based on the outcome (eating food, hitting obstacles, etc.).
5. The experience (state, action, reward, next state) is stored in memory.
6. The neural network is periodically trained on batches of stored experiences.

## Requirements

- Python 3.x
- PyTorch
- Pygame
- Matplotlib
- NumPy

## Usage

Run the `train.py` script to start training the AI:

```
python train.py
```

The training progress will be displayed in real-time, showing the game screen and a plot of scores over time.

## Future Improvements

- Implement prioritized experience replay
- Experiment with different network architectures
- Add support for different game modes or obstacles
