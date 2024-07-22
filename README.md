# AtariPongDQN
# Deep Q-Network (DQN) for Atari Pong
This repository contains the implementation of a Deep Q-Network (DQN), DDQN and PPO techniques to play the Atari Pong game using Reinforcement Learning techniques. The project demonstrates training a neural network to play the game and evaluates its performance.

## Table of Contents
Introduction
Project Structure
Usage
Training the Agent
Results

# Introduction:
This project aims to create an agent that can play the Atari Pong game using the Deep Q-Network (DQN) algorithm. The DQN algorithm combines Q-Learning with deep neural networks and experience replay to handle high-dimensional input spaces, such as game frames.

# Project Structure:
## (1)Root:
The '${ROOT} is described as below.

```plaintext
${ROOT}/
│
├── pongDQN.ipynb         # Python script for training and evaluating DQN technique on Pong
├── pongDDQN.ipynb        # Python script for training and evaluating DDQN technique on Pong
├── pongPPO.ipynb         # Python script for training and evaluating PPO technique on Pong
├── report.pdf            # Report Summarizing the results
├── README.md             # Project documentation
├── requirements.txt      # Python dependencies
├── checkpoint/           # Pre-trained weights and model parameters checkpoint directory
│   ├── ddqn2.pth         # Checkpoint for DDQN pre-trained weights and model parameters
│   ├── dqn.pth           # Checkpoint for DQN pre-trained weights and model parameters
├── videos/               # Pong Agent evaluation mode visualization 
│   ├── ddqnPong.mp4      # DDQN pong evaluation run
│   ├── dqnPong.mp4       # DQN pong evaluation run
└── requirements.txt      # Requirements file for model dependencies

## Usage:
To train the agent and evaluate its performance, follow these steps:

## Training the Agent:
Open the pongDQN.ipynb/ pongDDQN.ipynb/ pongPPO.ipynb notebook and run the cells to start the training process. The training process loads the pre-trained and further updates the model checkpoints after every 100 epochs and dynamically plots the training rewards.

# Key Components
Replay Buffer: Stores the agent's experiences to sample and train the network.
DQN/ DDQN Algorithm: Implements the Deep Q/ Double Deep Q-learning update rule using a neural network.
Training Loop: Iterates over episodes, collects experiences, updates the network, and tracks rewards.

# Evaluating the Agent:
After training, run the evaluation section of the notebook to see the agent's performance. The evaluation process loads the saved model and runs the agent in evaluation/ greedy mode.

# Results:
DQN


DDQN
