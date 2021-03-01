Deep Assist
===========

Create assistive agents to help humans with real-time control tasks.

Usage
-----

Install Python dependencies with the [pip](https://pip.pypa.io/en/stable/installing/) package
manager using

```
pip install -r requirements.txt
```

Install [gym](https://github.com/openai/gym) change the name of `deepassist/lunar_lander_for_{bots,humans}.py` to `deepassist/lunar_lander.py` and overide `gym/envs/box2d/lunar_lander.py`. It is the env for lunar lander. Recommand to read.

Install [baselines](https://github.com/openai/baselines) and replace `baselines/baselines/deepq/simple.py` with `deepassist/simple.py`. It is the deep q-learning method. Recommand to read.

Extract [this zip file](https://drive.google.com/file/d/1PWeF-OaX1EaKlyU3eQPwZOl8qv7qlmgL/view?usp=sharing) into `deepassist/`.

For the quadrotor experiments, install [ardrone_autonomy](https://wiki.ros.org/ardrone_autonomy) and [vicon_bridge](https://wiki.ros.org/vicon_bridge).

1.0-lunarlander-sim.ipynb : Use simulated pilots to train and evaluate.  
1.1-lunarlander-sim-analysis : Analyze the performance of the agents obtained in 1.0.  
1.2-lunarlander-human : Use really humans to train and evaluate.  
1.3-lunarlander-sim-analysis : Analyze the performance of the agents obtained in 1.2.  

Questions and comments
----------------------

Please contact the author at `sgr [at] berkeley [dot] edu` if you have questions or find bugs.

Citation
--------
If you find this software useful in your work, we kindly request that you cite the following [paper](https://arxiv.org/abs/1802.01744):

```
@InProceedings{Reddy/etal/18a,
  title={Shared Autonomy via Deep Reinforcement Learning},
  author={Reddy, Siddharth and Dragan, Anca D. and Levine, Sergey},
  booktitle={Arxiv 1802.01744},
  year={2018},
  url={https://arxiv.org/abs/1802.01744}
}
```
