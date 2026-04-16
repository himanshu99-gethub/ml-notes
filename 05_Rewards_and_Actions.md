# Rewards and Actions

## What are Rewards?
In reinforcement learning, rewards are the feedback received from the environment after taking an action. They guide the agent in learning the best actions to take in a given situation. A higher reward indicates a better action, while a lower or negative reward suggests that the action was not beneficial.

## Reward Functions
A reward function defines how rewards are assigned based on the agent's actions and the state of the environment. It is a critical component because it influences the learning process. The goal is to maximize the cumulative reward over time.

### Key Concepts:
- **Immediate Reward:** The reward received after taking an action.
- **Cumulative Reward:** The total reward accumulated over time, often considered in the context of discounting future rewards.

## Action Selection Strategies
Choosing the right action in a given state is crucial for effective learning. Some common strategies include:
- **Greedy Strategy:** Always choose the action that currently seems the best based on learned values.
- **Random Strategy:** Choose actions randomly to explore different possibilities.
- **Epsilon-Greedy Strategy:** A combination of the two, where most of the time the best-known action is chosen, and occasionally, a random action is taken to explore new possibilities.

### Epsilon-Greedy Strategy
In the epsilon-greedy strategy, we introduce a parameter ε (epsilon), which represents the probability of taking a random action. For instance:
- With a probability of (1 - ε), the agent selects the best-known action.
- With a probability of ε, the agent randomly selects an action.
This approach helps balance exploration (trying new actions to discover their rewards) and exploitation (leveraging known actions that yield high rewards).

## Exploration vs Exploitation
The exploration vs exploitation dilemma is a fundamental concept in reinforcement learning. 
- **Exploration:** Searching for new actions to discover their potential rewards. This is essential for learning about the environment.
- **Exploitation:** Utilizing known information to maximize rewards based on current knowledge. This can lead to short-term gains but may miss out on better long-term strategies.

Balancing these two is crucial for efficient learning and decision-making in uncertain environments.

## Examples
1. **Epsilon-Greedy Example:**
   - Suppose ε = 0.1, the agent will choose the best action 90% of the time and a random action 10% of the time. This keeps the agent learning while primarily focusing on actions that yield rewards.

2. **Reward Function Example:**
   - In a game, reaching a certain level could yield a reward of +10 points, while failing might give -5 points. The agent learns to maximize its score by understanding these reward functions.

By carefully designing reward functions and action selection strategies, we can train agents to perform optimally in various scenarios.