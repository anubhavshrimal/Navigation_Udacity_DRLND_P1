# Navigation_Udacity_DRLND_P1

Project done as part of the [Udacity Deep Reinforcement Learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893). The objective of this project is to create an Deep-Q Learning agent that is able to maximize the reward in the [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents) based [Banana Collector](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector) environment.

## Game Environment Details

![Game Environment](https://video.udacity-data.com/topher/2018/June/5b1ab4b0_banana/banana.gif)

The environment has an Agent in a square world which contains `yellow` and `blue` bananas. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

* `0` - move forward.
* `1` - move backward.
* `2` - turn left.
* `3` - turn right.

The environment is considered to be solved when the Agent gets an average score of +13 over 100 consecutive episodes.

**Note:** This project uses a simulator provided by Udacity which is similar but not identical to the Banana Collector environment on the [Unity ML-Agents GitHub page](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector).

## Getting Started

1. Install project dependencies by following the instructions mentioned in the [Installation_Guide.md](Installation_Guide.md).

2. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

3. Place the file in `/data` directory, and unzip the file.

## Instructions

Following are the steps to train your agent:

1. Clone this github repository:
   ```bash
    git clone https://github.com/anubhavshrimal/Navigation_Udacity_DRLND_P1.git
    cd Navigation_Udacity_DRLND_P1/
   ```
2. Activate the conda environment where you installed the dependencies and open jupyter notebooks. 
   ```bash
    conda activate drlnd
    jupyter notebook
   ```
3. Open `Navigation.ipynb` on your browser and run all the cells of the notebook.

## Files

* `checkpoint.pth` are the pre-trained model weights for the Agent, which can be used to further train the Agent or to see how the trained agent performs over the environment
* `Navigation.ipynb` is the ipython notebook which trains the Agent in the banana environment
* `dqn` folder contains the implementation for the `Agent` and the `Qnetwork`

## Algorithm

The algorithm and hyper-parameter details are mentioned in [Report.md](./Report.md).
