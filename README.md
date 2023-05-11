# OpenAI Gym Reinforcement Learning
Reinforcement Learning using Stable Baselines 3 with OpenAI Gym 

Gyms: Atari, Toy Text, Classic Control, Box2D

Stable Baselines 3: https://github.com/DLR-RM/stable-baselines
OpenAI Gym: https://github.com/openai/gym

For Stable Baseline 3:
1. Version "3." typo fix https://github.com/openai/gym/issues/3202#issuecomment-1510402359
2. Algorithm only supports ... as actions spaces but ... was provided (Gymnasium):
    import gymnasium as gym  
    import sys  
    sys.modules["gym"] = gym  

For OpenAI Gym ```pip install```:
1. pyglet==1.5.27 (name 'glPushMatrix' is not defined)
2. gym[atari, box2d, classic_control] (Probably not all since mujoko is not on Windows)

Note: Gymnasium, a fork of Gymnasium could be used? Need further testing with compabilities.  
Gymnasium: https://github.com/Farama-Foundation/Gymnasium  
For Gymnasium to work on Windows ```pip install```:
1. swig
2. gymnasium[all]
3. gymnasium[accept-rom-license]
4. shimmy

All codes are written from scratch based on documentation.