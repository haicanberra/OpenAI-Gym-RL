# Reinforcement-Learning
Reinforcement Learning using Stable Baselines 3 with OpenAI Gym 

Stable Baselines 3: https://github.com/DLR-RM/stable-baselines
OpenAI Gym: https://github.com/openai/gym

For Stable Baseline 3:
1. Version "3." typo fix https://github.com/openai/gym/issues/3202#issuecomment-1510402359
2. Algorithm only supports ... as actions spaces but ... was provided:
    import gymnasium as gym
    import sys
    sys.modules["gym"] = gym

For OpenAI Gym ```pip install```:
1. lockfile
2. gym[all]

Note: Gymnasium, a fork of Gymnasium could be used? Need further testing with compabilities.
Gymnasium: https://github.com/Farama-Foundation/Gymnasium
For Gymnasium to work on Windows ```pip install```:
0. swig
1. gymnasium[all]
2. gymnasium[accept-rom-license]
3. shimmy