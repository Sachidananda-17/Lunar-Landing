<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>
    <h1 style="text-align: center;">LunarLander RL Agent</h1>
        https://github.com/Sachidananda-17/Lunar-Landing/assets/107436781/a3743af8-e0e0-4417-bd14-be6ee32699a
    <p>This repository contains a Reinforcement Learning (RL) agent implemented in PyTorch to solve the LunarLander-v2 environment from the OpenAI Gym. The agent utilizes a Deep Q-Network (DQN) to learn how to control the lunar lander and safely land it on the moon's surface.</p>
    <h2>Overview</h2>
    <p>The LunarLander-v2 environment simulates the task of landing a spacecraft on the moon. The agent has control over the craft's main engine and orientation engines to maneuver and land safely. The goal is to learn a policy that maximizes the cumulative reward while safely landing on the designated landing pad.</p>
    <h2>Key Concepts and Components</h2>
    <ul>
        <li><strong>Deep Q-Network (DQN):</strong> The agent's neural network architecture is implemented using PyTorch. It consists of fully connected layers with ReLU activation functions.</li>
        <li><strong>Replay Memory:</strong> Experience replay is utilized to store and sample past experiences for efficient training. It helps stabilize and improve the learning process.</li>
        <li><strong>Target Network:</strong> A target Q-network is used to stabilize training by providing more stable target values during the learning process.</li>
        <li><strong>Epsilon-Greedy Exploration:</strong> The agent balances exploration and exploitation using an epsilon-greedy policy. It selects random actions with probability epsilon and greedy actions based on the learned Q-values otherwise.</li>
        <li><strong>Training Loop:</strong> The agent interacts with the environment, collects experiences, and updates its Q-network parameters using mini-batch gradient descent.</li>
    </ul>
    <h2>Metrics</h2>
    <ul>
        <li><strong>Average Score per Episode:</strong> The training process prints the average score achieved by the agent over the last 100 episodes. This metric indicates the agent's learning progress and performance.</li>
        <li><strong>Environment Solving:</strong> The environment is considered solved when the average score over the last 100 episodes exceeds 200. Upon solving, the training process stops, and the model parameters are saved.</li>
    </ul>
    <h2>Installation and Usage</h2>
    <p>To run the RL agent and train it to solve the LunarLander-v2 environment, follow these steps:</p>
    <ol>
        <li>Clone this repository to your local machine.</li>
        <li>Install the required dependencies by executing the following command:</li>
    </ol>
    <pre><code>pip install gym gym[atari,accept-rom-license] box2d torch</code></pre>
    <p>Ensure you have the necessary dependencies installed, including Gym and PyTorch, to execute the code successfully.</p>
    <h2>Getting Started</h2>
    <p>To begin training the RL agent, execute the provided code in your preferred Python environment. Adjust hyperparameters and training settings as needed for your specific requirements.</p>
    <h2>License</h2>
    <p>This project is licensed under the <a href="LICENSE">MIT License</a>.</p>
</body>
</html>
