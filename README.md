

# Train a double-jointed arm to move to target locations

## Project Details


This project work with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment, in the environment, a double-jointed arm can move to target locations and the environment contains 20 identical agents, each with its own copy of the environment.
A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of the agent is to maintain its position at the target location for as many time steps as possible.
The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The environment is considered solved when the agents get an average score of +30 (over 100 consecutive episodes, and over all agents),  Specifically:

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 20 (potentially different) scores. We then take the average of these 20 scores.
- This yields an average score for each episode (where the average is over all 20 agents).


## Getting Started

#### Instructions for installing dependencies or downloading needed files.


To set up your python environment to run the code in this repository, follow the instructions below.

1. Create (and activate) a new environment with Python 3.6.

	- __Linux__ or __Mac__:
	```bash
	conda create --name drlnd python=3.6
	source activate drlnd
	```
	- __Windows__:
	```bash
	conda create --name drlnd python=3.6
	activate drlnd
	```

2. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.  
	- Next, install the **classic control** environment group by following the instructions [here](https://github.com/openai/gym#classic-control).
	- Then, install the **box2d** environment group by following the instructions [here](https://github.com/openai/gym#box2d).

3. Clone the repository (if you haven't already!), and navigate to the `python/` folder.  Then, install several dependencies.
```bash
git clone https://github.com/udacity/deep-reinforcement-learning.git
cd deep-reinforcement-learning/python
pip install .
```

4. Create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `drlnd` environment.  
```bash
python -m ipykernel install --user --name drlnd --display-name "drlnd"
```

5. Before running code in a notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu.

![Kernel][image/choose_kernel.png]


#### Instructions for prepare the environment


1. Download the environment from the links below(for this project, there is no need to install Unity). You need only select the environment that matches your operating system:
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

2. Place the file in the GitHub repository, and unzip (or decompress) the file.


## Instructions

#### Instructions for how to run the code in the repository, to train the agent.


Step 1: Activate the Environment

- __Linux__ or __Mac__:
```bash
source activate drlnd
```
- __Windows__:
```bash
activate drlnd
```


Step 2: Open the project file


```bash
jupyter notebook Continuous_Control.ipynb
```

Before running code in the notebook, change the kernel to match the `drlnd` environment by using the drop-down `Kernel` menu.


Step 3: Watch a smart agent

- 1. Start the environment
- 2. Examine the State and Action Spaces¶
- 4. Watch a Smart Agent!

Step 4: Train the agent

- 1. Start the environment
- 2. Examine the State and Action Spaces¶
- 3. Train the Agent with DDPG

## References

* Udacity's [Deep Reinforcement Learning Nanodegree program](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) repository, https://github.com/udacity/deep-reinforcement-learning
* [MorvanZhou's video course](https://github.com/MorvanZhou)
* Continuous control with deep reinforcement learning from Deep mind:[arXiv:1509.02971 ](https://arxiv.org/abs/1509.02971)
