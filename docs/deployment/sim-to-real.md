# Sim-to-Real Transfer, Safety & Reliability

## Overview

Evaluate the real-world validity and operational risks of robot policies.

This topic guide identifies concepts to explore and an experiment to try. Use the linked documentation for implementation details.

## Prerequisites

[Physics Simulation & Robot Modeling](../simulation/physics.md), [Robot Control & Motion Planning](control-and-planning.md), [Edge AI Inference & Model Deployment](edge-inference.md)

## Key concepts

- Reality gap.
- system identification.
- domain adaptation/randomization.
- camera/actuator alignment.
- latency compensation.
- safety constraints and supervised testing.
- failure recovery.
- reproducible reliability benchmarks.

## Try it

Conduct a staged sim-to-real trial; record real-world task success and intervention rates; identify failure modes and implement appropriate constraints.

Record your setup, inputs, measurements, and failure cases. Keep the experiment small enough to repeat, and compare the result against a simple baseline.

## Further reading

- [ROS 2 documentation](https://docs.ros.org/)
- [LeRobot](https://github.com/huggingface/lerobot)

## Next steps

- Apply this topic in the [SO-101 project](../projects/so101.md).
