# Introduction

This course focuses on easy to use theory and practicle through collab notebooks \
[https://huggingface.co/learn/deep-rl-course/unit0/introduction](https://huggingface.co/learn/deep-rl-course/unit0/introduction)

All models will be pushed into huggingface and can be seen in [Leaderboard](https://huggingface.co/spaces/huggingface-projects/Deep-Reinforcement-Learning-Leaderboard), to search for model used in this repo select ENV, type pankajr141 under userid and click "Search My models" 

# Model collection
Below link contains the location where all model build using this repo are stored

[Hugging Face Model Collection for this course](https://huggingface.co/collections/pankajr141/huggingface-deeprl-6780de9f81e69ba91aee9019)

# Notebooks

* [Unit 1 - Introduction to Deep Reinforcement Learning](https://nbviewer.org/github/pankajr141/courses/blob/main/Deep%20RL%20-%20Hugging%20Face/notebooks/unit1/unit1.ipynb) \
Initial Unit to interact with gymnasium env ang train a PPO model using stablebaseline3
> <b>Env -</b> [LunarLander-v2](https://gymnasium.farama.org/environments/box2d/lunar_lander/) \
> <b>Env-Lib -</b> [gymnasium](https://gymnasium.farama.org/) \
> <b>RL-Algo -</b> [PPO](https://stable-baselines3.readthedocs.io/en/master/modules/ppo.html) \
> <b>RL-Lib -</b> [stable_baselines3](https://stable-baselines3.readthedocs.io/en/master/index.html)

* [Unit 1 Bonus - Introduction to Deep Reinforcement Learning with Huggy](https://nbviewer.org/github/pankajr141/courses/blob/main/Deep%20RL%20-%20Hugging%20Face/notebooks/unit1_bonus.ipynb) \
Bonus unit where we interact with Unity based Env and train RL model using PPO
> <b>Env -</b> [Huggy](https://github.com/huggingface/Huggy) \
> <b>Env-Lib -</b> Unity \
> <b>RL-Algo -</b> PPO \
> <b>RL-Lib -</b> [MLAgents](https://github.com/Unity-Technologies/ml-agents)

* [Unit 2 - Introduction to Q Learning](https://nbviewer.org/github/pankajr141/courses/blob/main/Deep%20RL%20-%20Hugging%20Face/notebooks/unit2.ipynb) \
Trains a Q-function, an action-value function encoded, in internal memory, by a Q-table containing all the state-action pair values.
<pre>
<b>Value-based method:</b> finds the optimal policy indirectly by training a value or action-value function that will tell us the value of each state or each state-action pair.
<b>TD approach:</b> updates its action-value function at each step instead of at the end of the episode.'
<b>Off-policy:</b> using a different policy for acting (inference) and updating (training).
</pre>
> <b>Env -</b> [FrozenLake-v1](https://gymnasium.farama.org/environments/toy_text/frozen_lake/), [Taxi-v3](https://gymnasium.farama.org/environments/toy_text/taxi/)\
> <b>Env-Lib -</b> [gymnasium](https://gymnasium.farama.org/) \
> <b>RL-Algo -</b> Q-Learning - Value based\
> <b>RL-Lib -</b> python and numpy

* [Unit 3 - Deep Q-Learning with Atari Games](https://nbviewer.org/github/pankajr141/courses/blob/main/Deep%20RL%20-%20Hugging%20Face/notebooks/unit3.ipynb) \
Trains a DQN model, uses Experiance Replay Buffer, Fixed Q Target uses 2 models, Double DQN i.e model 1 for action estimation and 2 for estimating value for corresponding action.
<pre>
<b>Experience Replay:</b> replay buffer to store previous episodes for retraining
<b>Fixed Q-Target:</b> separate N/W for Q-Target and Q-value, to avoid issue of chasing a moving target.
<b>Double DQN:</b> handle overestimation of Q values. This solution uses two networks to decouple the action selection from the target Value generation.
    <b>DQN Network</b> to select the best action to take for the next state (the action with the highest Q-Value)
    <b>Target Network</b> to calculate the target Q-Value of taking that action at the next state. This approach reduces the Q-Values overestimation, it helps to train faster and have more stable learning.
</pre>
> <b>Env -</b> [SpaceInvadersNoFrameskip-v4](https://ale.farama.org/environments/space_invaders/) \
> <b>Env-Lib -</b> [gymnasium](https://gymnasium.farama.org/) \
> <b>RL-Algo -</b> DQN - Value based\
> <b>RL-Lib -</b> [rl-baselines-zoo](https://github.com/DLR-RM/rl-baselines3-zoo) - wrapper on top of stable_baselines3

* [Unit 4 - Policy Gradient with PyTorch](https://nbviewer.org/github/pankajr141/courses/blob/main/Deep%20RL%20-%20Hugging%20Face/notebooks/unit4.ipynb) \
Trains a DQN model, uses Experiance Replay Buffer, Fixed Q Target uses 2 models, Double DQN i.e model 1 for action estimation and 2 for estimating value for corresponding action.
<pre>
<b>Policy Based</b> directly learb from optimal policy without learning value function
</pre>
> <b>Env -</b> [CartPole-v1](https://www.gymlibrary.dev/environments/classic_control/cart_pole/), [Pixelcopter-PLE-v0](https://pygame-learning-environment.readthedocs.io/en/latest/user/games/pixelcopter.html) \
> <b>Env-Lib -</b> [gymnasium](https://gymnasium.farama.org/) \
> <b>RL-Algo -</b> Monte Carlo Reinforce - Policy based \
> <b>RL-Lib -</b> Pytorch - Custom implementation
