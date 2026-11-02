# Reinforcement Learning for Robotics

## Overview

Learn action policies through interaction and feedback.

This topic guide identifies concepts to explore and an experiment to try. Use the linked documentation for implementation details.

## Prerequisites

[Deep Learning with PyTorch](../foundations/pytorch.md), [Robot Kinematics & Dynamics](../simulation/kinematics-and-dynamics.md)

## Key concepts

- MDPs, observations/states/actions/rewards.
- value functions and Bellman equations.
- policy gradients and actor–critic.
- PPO and SAC.
- reward design.
- exploration.
- continuous control and generalization.

## Try it

Define a task with rewards and terminations; train a policy; compare returns, task success, and performance on unseen scenarios.

Record your setup, inputs, measurements, and failure cases. Keep the experiment small enough to repeat, and compare the result against a simple baseline.

## Further reading

- [LeRobot](https://github.com/huggingface/lerobot)
- [Isaac Lab documentation](https://isaac-sim.github.io/IsaacLab/)

## Next steps

- [World Models & Predictive Learning](world-models.md)
- [Robot Policy Training with Isaac Lab](isaac-lab.md)
