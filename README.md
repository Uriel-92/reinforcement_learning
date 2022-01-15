Neural network that plays Super Mario. The goal is to train a neural network known as Proximal Policy Optimization (PPO) to learn how to play Super Mario. The python package used is stable baseline and can be found on this webpage https://stable-baselines.readthedocs.io/en/master/modules/ppo2.html . This neural network was trained for a million iterations and the first level was passed. However, if you want to pass the next level you should train for more times. 

Python package used
Neural network 

-import os
-from stable_baselines3 import PPO
-from stable_baselines3.common.callbacks import BaseCallback

For play Super Mario and visualize the frames

from gym.wrappers import GrayScaleObservation
from stable_baselines3.common.vec_env import VecFrameStack, DummyVecEnv
from matplotlib import pyplot as plt
import gym_super_mario_bros
from nes_py.wrappers import JoypadSpace
from gym_super_mario_bros.actions import SIMPLE_MOVEMENT
