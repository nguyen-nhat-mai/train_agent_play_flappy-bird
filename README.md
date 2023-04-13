# TRAIN AGENTS TO PLAY TEXT FLAPPY BIRD
This project is a part of Reinforcement Learning course at CentraleSupelec
## Project description
The project focuses on using reinforcement learning to train agents to play a text-based version of the popular video game, Flappy Bird. The goal is to find the optimal policy that maximizes the cumulative reward over time. Two reinforcement learning algorithms, Q-learning and SARSA, will be used and compared in terms of their performance in reward and convergence time. This project provides hands-on experience in reinforcement learning.

## Environment
TextFlappyBird-v0 is a simplified version of Flappy Bird where the player controls a bird with the '@' character, navigating it through gaps in pipes represented by '|' moving from right to left. The objective is to take either "Idle" or "Flap" action, and the game ends when the bird collides with a pipe or hits the ground represented by '^'. The environment provides the state of the game, which includes horizontal and vertical distance to the pipeline gap center, and the reward returned is 1 if the bird is still alive.

![image](https://user-images.githubusercontent.com/85484281/231840250-02e097f5-a990-4452-8a19-85962fe5e788.png)

## Agents
Q-learning: Q(s,a) ← (1 - α) Q(s,a) + α [r + γ max(Q(s',a'))]

SARSA: Q(s,a) ← (1 - α) Q(s,a) + α [r + γ Q(s',a')]

where Q(s,a) is the estimated action-value function for state s and action a, α is the learning rate, r is the immediate reward received after taking action a in
state s, γ is the discount factor, s' is the next state, and a' is the next action.
