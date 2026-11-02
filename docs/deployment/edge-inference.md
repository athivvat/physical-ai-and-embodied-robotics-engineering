# Edge AI Inference & Model Deployment

## Overview

Serve learning models under the compute and timing constraints of robot platforms.

This topic guide identifies concepts to explore and an experiment to try. Use the linked documentation for implementation details.

## Prerequisites

[Deep Learning with PyTorch](../foundations/pytorch/index.md), [ROS 2 & Robot Software Architecture](ros2.md)

## Key concepts

- ONNX/model export.
- TensorRT.
- quantization and reduced precision.
- latency, throughput and memory.
- asynchronous inference.
- Jetson/Isaac ROS.
- monitoring and model rollback.

## Try it

Deploy and profile an inference pipeline; measure end-to-end latency; document accuracy–latency trade-offs and operational monitoring.

Record your setup, inputs, measurements, and failure cases. Keep the experiment small enough to repeat, and compare the result against a simple baseline.

## Further reading

- [ROS 2 documentation](https://docs.ros.org/)
- [LeRobot](https://github.com/huggingface/lerobot)

## Next steps

- [Sim-to-Real Transfer, Safety & Reliability](sim-to-real.md)
