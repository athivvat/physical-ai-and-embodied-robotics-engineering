# World Models & Predictive Learning

## Overview

Learn predictive models of physical transitions and use them for reasoning or planning. A world model may use Transformers, recurrent state-space models, or other architectures; it is not synonymous with a physics simulator.

This topic guide identifies concepts to explore and an experiment to try. Use the linked documentation for implementation details.

## Prerequisites

[Transformers & Attention Architectures](../foundations/transformers.md), [Reinforcement Learning for Robotics](reinforcement-learning.md)

## Key concepts

- Forward/inverse dynamics.
- state-space and latent-state models.
- RSSM.
- action-conditioned prediction.
- model-based RL.
- model predictive control.
- video/world foundation models.
- NVIDIA Cosmos case studies.
- epistemic uncertainty and rollout error.

## Try it

Predict next states given current state and action; evaluate multi-step error; use a learned transition model to compare candidate actions in a bounded task.

Record your setup, inputs, measurements, and failure cases. Keep the experiment small enough to repeat, and compare the result against a simple baseline.

## Further reading

- [NVIDIA Cosmos](https://docs.nvidia.com/cosmos/)
- [Isaac Lab documentation](https://isaac-sim.github.io/IsaacLab/)

## Next steps

- Apply this topic in the [SO-101 project](../projects/so101.md).
