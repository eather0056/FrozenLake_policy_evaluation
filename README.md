# FrozenLake Policy Evaluation

## Overview
This project implements various reinforcement learning techniques to evaluate and improve policies on the "FrozenLake" environment from OpenAI's gym. Supervised by Prof. Ricard Marxer at the University of Toulon, this project explores the application of Markov Decision Processes (MDP), policy evaluation methods, action-value function computation, epsilon-greedy policies, SARSA, and Q-learning to navigate through the stochastic environment of FrozenLake.
### Google Colab
[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mC3VPcRjybNgTIZkVBzsnvGaVaC--HSk#scrollTo=qL6xBo8Lg-gT)
## Methods Implemented
- **MDP from Gym Environment**: Utilization of the gym environment to model the FrozenLake as a Markov Decision Process.
- **Policy Evaluation**: Implementation of various value function estimation methods:
  - Direct Method using the environment's transition probabilities (P) and rewards (R).
  - Naive Method that assumes the possibility of setting an arbitrary initial state.
  - Monte Carlo Methods for policy evaluation.
  - Time-Difference (TD) Method for value function estimation.
- **Action-Value Function**: Computation of the action-value function using methods such as:
  - Naive Method (assuming control over the initial state).
  - Monte Carlo "first visit" and "every visit" methods.
  - Monte Carlo incremental method.
  - TD learning.
- **Epsilon-Greedy Policy**: Implementation of an epsilon-greedy policy to balance exploration and exploitation, with different behaviors in training and evaluation modes.
- **SARSA (State-Action-Reward-State-Action)**: Implementation of the SARSA algorithm for policy learning, leveraging TD estimation of action-value functions and epsilon-greedy policy.
- **Q-Learning**: Implementation of Q-learning, an off-policy TD control algorithm, assuming an optimal policy for updating action-values.

## Project Structure
- `envs/`: Directory containing custom environments or wrappers for the FrozenLake gym environment.
- `agents/`: Implementation of various reinforcement learning agents (SARSA, Q-learning, etc.).
- `policies/`: Epsilon-greedy and other policy implementations.
- `utils/`: Utility functions for state representation, reward processing, and other helper functions.
- `main.py`: The main script to run experiments and evaluate policies.
- `requirements.txt`: List of dependencies for the project.

## Setup
To set up the project environment, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/eather0056/FrozenLake_policy_evaluation.git
   ```
2. Navigate to the project directory:
   ```
   cd FrozenLake_policy_evaluation
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage
To run experiments and evaluate the policies on the FrozenLake environment, execute the `main.py` script:
```
python main.py
```

## Results
The project includes detailed experimentation with various reinforcement learning techniques to understand their performance in the FrozenLake environment. Results include policy effectiveness, convergence analysis, and comparison between different methods.

## Acknowledgments
Special thanks to Prof. Ricard Marxer for guidance and supervision throughout the project, and to the contributors and OpenAI for the gym environment.
