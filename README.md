# Learning to Win: Deep Reinforcement Learning in Board Games
## Project Overview

This project investigates the use of **Deep Reinforcement Learning (DRL)** to train agents to play two classic board games: **Tic-Tac-Toe** and **Connect Four**. Using neural networks implemented in **PyTorch**, agents learn optimal strategies through self-play and reward-based feedback rather than predefined rules.

The project demonstrates how reinforcement learning scales from a simple environment (Tic-Tac-Toe) to a more complex one (Connect Four), highlighting differences in state representation, action spaces, and learning difficulty.

## Motivation

Board games offer structured environments that are ideal for studying reinforcement learning.
By working with both Tic-Tac-Toe and Connect Four, we aim to:
* Compare learning behavior across games with different complexity levels
* Explore how state and action space size affects training
* Understand how neural-network-based agents improve decision-making through experience
Tic-Tac-Toe serves as a baseline environment, while Connect Four introduces deeper strategy and longer-term planning.

## Games Implemented
### Tic-Tac-Toe
* Board size: 3 × 3
* State representation:
    * X = 1
    * O = -1
    * Empty = 0

* Action space: 9 possible moves

### Connect Four
* Board size: 6 × 7
* State representation:
    * Player 1 = 1
    * Player 2 = -1
    * Empty = 0

* Action space: 7 possible columns
* More complex win conditions and longer game horizons


## Methods
**Model Architecture**:
* Fully connected neural networks
* Inputs represent the current board state
* Outputs represent action values for each possible move
**Learning Approach**:
* Reinforcement learning via self-play
* Rewards assigned for wins, losses, and draws
* Invalid actions penalized
**Training Framework**: PyTorch

## Technologies Used
* Python
* PyTorch
* NumPy
* Matplotlib
* Google Colab Notebook

## Results
Across training episodes, agents show clear performance improvements:
* Reduction in invalid or suboptimal moves
* Increased win and draw rates
* More consistent strategic behavior over time

The Connect Four agent required significantly more training due to the larger state and action space, illustrating the added complexity of deeper decision trees.

Visualizations in the notebook track learning progress and performance trends.
