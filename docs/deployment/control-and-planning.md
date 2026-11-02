# Robot Control & Motion Planning

## Overview

Convert intentions and learned actions into feasible, bounded robot motions.

This topic guide identifies concepts to explore and an experiment to try. Use the linked documentation for implementation details.

## Prerequisites

[Robot Kinematics & Dynamics](../simulation/kinematics-and-dynamics.md)

## Key concepts

- Feedback/PID.
- joint and Cartesian control.
- interpolation and trajectory generation.
- RRT/RRT* and optimization-based planning.
- collision avoidance.
- MPC.
- safety wrappers for learned policies.

## Try it

Plan and execute constrained motions; enforce workspace and joint limits; compare classical control with learned policies.

Record your setup, inputs, measurements, and failure cases. Keep the experiment small enough to repeat, and compare the result against a simple baseline.

## Further reading

- [ROS 2 documentation](https://docs.ros.org/)
- [LeRobot](https://github.com/huggingface/lerobot)

## Next steps

- [Sim-to-Real Transfer, Safety & Reliability](sim-to-real.md)
