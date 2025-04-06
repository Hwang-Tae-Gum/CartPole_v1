# Deep Q-Network (DQN) for CartPole-v1

## Description
- This project implements a **Deep Q-Network (DQN)** agent to solve the CartPole-v1 environment using **PyTorch** and **Gymnasium**. 
- The code includes functionalities for training, optimizing, and validating the model, as well as saving and visualizing results. 
### Key features include:
- Replay Memory for storing transitions.
- Epsilon-greedy policy for action selection.
- Target network updates using soft updates.
- Visualization of training metrics (durations, losses, epsilon decay).
- Saving the trained model to Google Drive.
- Recording and displaying videos of the agent's performance.

## Dataset Information
This is a reinforcement learning project, so no dataset is used. Instead, the agent interacts directly with the CartPole-v1 environment to collect experience.

## Model Architecture
The DQN model architecture is defined as follows:
- **Input Layer**: Matches the size of the state space (number of observations).
- **Hidden Layer 1**: 128 neurons with ReLU activation.
- **Hidden Layer 2**: 64 neurons with ReLU activation.
- **Output Layer**: Matches the size of the action space (number of possible actions).

## Hyperparameters
The following hyperparameters are used in this implementation:
- **Batch Size**: 128
- **Discount Factor (Gamma)**: 0.99
- **Epsilon Start**: 0.9
- **Epsilon End**: 0.05
- **Epsilon Decay**: 300
- **Soft Update Factor (Tau)**: 0.01
- **Learning Rate**: \(1 \times 10^{-4}\)

## Improvements and Future Updates
To enhance the current implementation, the following improvements and updates are suggested:
1. Implement **Prioritized Experience Replay** to improve sampling efficiency.
2. Add support for other environments to generalize the agent's capabilities.
3. Use **Double DQN** to reduce overestimation bias.
4. Incorporate a **Dueling DQN architecture** for better value estimation.
5. Add more visualizations, such as reward trends and Q-value distributions.
6. Provide a command-line interface for easier configuration and execution.
7. Include unit tests to ensure code reliability.

## Result Video Link
You can check the performance of the trained agent in the following YouTube video:
[https://www.youtube.com/watch?v=doFdPc1L1zw](https://www.youtube.com/watch?v=doFdPc1L1zw)


## Conclusion
- This project demonstrates a successful implementation of a DQN agent for solving the CartPole-v1 environment. 
- The model effectively learns to balance the pole through reinforcement learning techniques and provides visual insights into its training process.
- Future updates can further enhance its robustness and generalizability to other environments or tasks.
