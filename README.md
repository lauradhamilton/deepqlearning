# Deep Q Learning Tutorial

In this tutorial, I will walk you through how to use Deep Q Learning to create an AI that learns visually (from pixels) and learns how to drive, solving CarRacing-v0. This software can be adapted with tuning to solve a wide variety of reinforcement learning problems.

# Resources
1. Read the seminal paper [Playing Atari with Deep Reinforcement Learning](https://www.cs.toronto.edu/~vmnih/docs/dqn.pdf) written by the [Deepmind](https://deepmind.com/) team.
2. Adapted from [Deep Q-Learning with Keras and Gym](https://keon.io/deep-q-learning/)
3. Uses the [Open AI Gym](https://gym.openai.com/) set of reinforcement learning libraries

# Language
We will use Python 2.7. Check that you have python installed:
```python```


# Libraries
We will use [gym](https://gym.openai.com/) for the [CarRacing-v0 environment](https://gym.openai.com/envs/CarRacing-v0/), [random](https://docs.python.org/2/library/random.html) for making explore/exploit decisions, [numpy](http://www.numpy.org/) for array manipulation, [collections](https://docs.python.org/2/library/collections.html) for storing our "memory" of past states, and [keras](https://keras.io/) for creating the neural nets.

# Install the libraries if you do not already have them installed
```
pip install gym
pip install keras
pip install tensorflow
```

# Now for the code. Let's start by importing the libraries we will need:
```
import gym
import random
import numpy
from collections import deque
from keras.models import Sequential
from keras.layers import Dense
from keras.optimizers import Adam
```