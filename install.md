# MADDPG-pytorch Install Tutorial

## Preparation

conda create -n maddpg python=3.6

conda activate maddpg

conda install tensorflow-gpu==1.15


## MADDPG

git clone https://github.com/Ray0117/maddpg-pytorch.git --recurse-submodules

sudo apt-get update && sudo apt-get install cmake libopenmpi-dev python3-dev zlib1g-dev

## Baseline

cd baselines

pip install -e .

// if there are errors about MuJoCo, just ignore it

## Multi-Agent Particle Environment

git clone https://github.com/Ray0117/multiagent-particle-envs.git

cd multiagent-particle-envs

pip install -e .

## PyTorch

conda install pytorch cudatoolkit=10.1 -c pytorch

## Necessary Dependencies

pip install seaborn pyglet==1.3.2 gym==0.9.4 //gym version must be 0.9.4

## TEST

cd maddpg-pytorch

python main.py --help //test if its ok

python main.py adv test
