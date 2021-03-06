# Learning to Guide: Guidance Law Based on Deep Meta-learning and Model Predictive Path Integral Control

### About


This work aims at implementing Model-based Deep Reinforcement Learning with Model Predictive Path Integral controller for the **missile guidance** problem as described in our paper
[Learning to Guide: Guidance Law Based on Deep Meta-learning and Model Predictive Path Integral Control](https://ieeexplore.ieee.org/document/8682051)
This IEEE Access paper is open access at https://ieeexplore.ieee.org/document/8682051 and also available on arXiv at https://arxiv.org/abs/1904.06892


### Dependencies

This code has been tested on python and requires tensorflow-gpu & numpy installed.
This demonstrative run is built on the pre-trained guidance neural network model, the code, system model and training dataset of which will be posted afterwards if anybody asks.

### How to Run

Please use `mppi_run.py` to run.

Run can also be done using `monte_carlo_simu.sh` to do iteratively runs to get Monte Carlo sampling results. In the paper the results
of Monte Carlo simulation are collected using the get_Monte.m file of MATLAB.

## Citing

If you find our works useful in your research, please consider citing:

```

@article{liang2019learning,
  title={Learning to Guide: Guidance Law Based on Deep Meta-Learning and Model Predictive Path Integral Control},
  author={Liang, Chen and Wang, Weihong and Liu, Zhenghua and Lai, Chao and Zhou, Benchun},
  journal={IEEE Access},
  volume={7},
  pages={47353--47365},
  year={2019},
  publisher={IEEE}
}
```

### File list

cost_functions.py       : define the cost function of MPPI controller.

neural_dynamics_dense.py: The neural network dynamic model with meta-learning online adaption built in.

get_Monte.m             : A simple MATLAB file to collect Monte Carlo simulation results.

inner_loop.py           : A look at the inner-loop dynamics in semi-physical simulation which is not included in this code set.

mppi_controller.py      : MPPI controller

mppi_run.py             : main file for simulation

monte_carlo_simu.sh     : Monte Carlo simulation

missile_env.py          : Guidance Environment


