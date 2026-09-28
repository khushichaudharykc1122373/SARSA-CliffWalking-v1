# SARSA Reinforcement Learning – CliffWalking-v1

## 📌 Project Overview

This project implements the **SARSA (State-Action-Reward-State-Action)** reinforcement learning algorithm using the **CliffWalking-v1** environment from Gymnasium.

SARSA is an **on-policy Temporal Difference (TD) learning algorithm** that learns the optimal action-selection policy through interaction with the environment. The agent updates its Q-values based on the current state, current action, reward, next state, and next action.

## 🎯 Objective

The main objective of this project is to understand and implement the **SARSA algorithm** and observe how an agent learns to navigate through the CliffWalking-v1 grid environment while avoiding the cliff and reaching the destination.

## 🌍 Environment

The project uses:

**CliffWalking-v1**

CliffWalking is a grid-world environment where the agent starts at a fixed position and must reach the goal while avoiding the cliff. Falling from the cliff results in a large negative reward.

## 🔄 Workflow

1. Create the `CliffWalking-v1` environment.
2. Initialize the Q-table.
3. Define the epsilon-greedy action-selection strategy.
4. Set SARSA parameters such as learning rate and discount factor.
5. Run multiple training episodes.
6. Select an action based on the current policy.
7. Take an action in the environment.
8. Observe the reward and next state.
9. Select the next action using the epsilon-greedy policy.
10. Update the Q-value using the SARSA update rule.
11. Repeat until the episode terminates.
12. Evaluate the learned policy.

## 🧠 SARSA Algorithm

SARSA updates the Q-value using:

```text
Q(s,a) ← Q(s,a) + α [r + γ Q(s',a') − Q(s,a)]
```

Where:

* **s** → Current state
* **a** → Current action
* **r** → Reward received
* **s'** → Next state
* **a'** → Next action
* **α** → Learning rate
* **γ** → Discount factor

## 🔑 Key Concepts

* Reinforcement Learning
* SARSA Algorithm
* Temporal Difference Learning
* Q-Learning / Q-Table concepts
* Epsilon-Greedy Policy
* Exploration vs. Exploitation
* State and Action
* Reward
* Learning Rate
* Discount Factor
* Policy Learning
* Gymnasium Environments

## 🛠️ Technologies Used

* Python
* NumPy
* Gymnasium
* Jupyter Notebook

## 📂 Project Structure

```text
SARSA-CliffWalking-v1/
│
├── SARSA_CliffWalking.ipynb
├── README.md
└── requirements.txt
```

## ⚙️ Installation

Install the required libraries:

```bash
pip install numpy gymnasium
```

## ▶️ How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Open `SARSA_CliffWalking.ipynb` in Jupyter Notebook or JupyterLab.
4. Run the cells sequentially.
5. Observe the learning process of the SARSA agent.

## 📊 Learning

During training, the agent gradually improves its action selection by updating the Q-table based on the rewards received from the environment.

The epsilon-greedy strategy allows the agent to balance:

* **Exploration** — trying different actions.
* **Exploitation** — selecting actions that currently have higher Q-values.

## 🎯 Learning Outcome

Through this project, I gained practical understanding of:

* How reinforcement learning agents interact with environments.
* How Q-tables represent state-action values.
* How SARSA performs on-policy Temporal Difference learning.
* How epsilon-greedy strategies handle exploration and exploitation.
* How an agent learns a policy through repeated interaction with an environment.

## 👩‍💻 Author

**Khushi Chaudhary**

B.Tech CSE | AI/ML Learner
