# AtariPongDQN
# Deep Q-Network (DQN) for Atari Pong
This repository contains the implementation of a Deep Q-Network (DQN), DDQN and PPO techniques to play the Atari Pong game using Reinforcement Learning techniques. The project demonstrates training a neural network to play the game and evaluates its performance.

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
```

## Usage:
To train the agent and evaluate its performance, follow these steps:

## Training the Agent:
Open the pongDQN.ipynb/ pongDDQN.ipynb/ pongPPO.ipynb notebook and run the cells to start the training process. The training process loads the pre-trained checkpoints and iteratively updates the model checkpoints after every 100 epochs. The training progress is dynamically plotted as a function of Total reqards in an episode vs the episode number.

# Key Components
Replay Buffer: Stores the agent's experiences to sample and train the network.
DQN/ DDQN Algorithm: Implements the Deep Q/ Double Deep Q-learning update rule using a neural network.
Training Loop: Iterates over episodes, collects experiences, updates the network, and tracks rewards.

# Evaluating the Agent:
After training, run the evaluation section of the notebook to see the agent's performance. The evaluation process loads the saved model and runs the agent in evaluation/ greedy mode.

# Results:
DQN
![dqnPong](https://github.com/user-attachments/assets/46946734-4d1d-424d-bbc6-b5f80bff81d7)
Pong A.I. RL DQN agent wins the match with a 21-11 score. 
![DQN Evaluation Run Rewards](https://github.com/user-attachments/assets/d131845a-2731-489b-9212-b65df96b7730)
Pong A.I RL agent which is in green is getting positive rewards as can be seen from attached evaluation run graph.

DDQN
![ddqnPong](https://github.com/user-attachments/assets/eb68a516-5668-4c2e-a182-2080927c655e)
Pong A.I. RL DQN agent wins the match with a 21-14 score. 

The better performance of DQN agent when compared to DQN agent is attributed to the fact that DDQN agent was trained only for 6000 episode while DQN agent was trained for 14000 episodes.

## Acknowledgment
This project uses computing resources from UB CCR and under the guidance of Prof. Alina Vereshchaka, Assistant Professor of Teaching at University at Buffalo.

