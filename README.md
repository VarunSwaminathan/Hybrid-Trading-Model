## Overview
This project focuses on developing a hybrid trading model that combines a Transformer-based feature extractor with a Proximal Policy Optimization (PPO) policy network. The goal of this model is to generate actionable trading signals—Buy, Sell, or Hold—by learning from historical market data. The model leverages the strengths of deep learning and reinforcement learning to capture complex temporal patterns and optimize trading decisions.

## Model Architecture
Transformer Feature Extractor: Captures temporal dependencies in the market data using self-attention mechanisms.
PPO Policy Network: Uses the extracted features to make decisions on whether to Buy, Sell, or Hold.
Hybrid Model: Combines the Transformer and PPO networks, feeding the features extracted by the Transformer into the PPO policy network.

## Fine-Tuning Details
The model has been fine-tuned using several optimization techniques:
Learning Rate Scheduling: Reduces the learning rate when the model's performance plateaus.
Early Stopping: Stops training when there is no improvement over a set number of epochs.
Gradient Clipping: Prevents exploding gradients by capping the gradients during backpropagation.

## Evaluation Metrics
The model is evaluated based on:
Cumulative Reward: The total reward accumulated during the simulation, indicating the model's overall performance.
Trade Logs: Detailed logs of each trade, including the action taken, execution price, and reward.
Trading Blotter: A simulated environment that provides a realistic assessment of the model's trading strategy.
