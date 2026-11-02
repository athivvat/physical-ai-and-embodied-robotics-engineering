# Vision-Language-Action Models

## Overview

Study models connecting perception and natural-language instructions to robot actions.

This topic guide identifies concepts to explore and an experiment to try. Use the linked documentation for implementation details.

## Prerequisites

[Transformers & Attention Architectures](../foundations/transformers.md), [Generative Models & Foundation Models](../foundations/generative-models.md), [Imitation Learning & Robot Demonstrations](imitation-learning.md)

## Key concepts

- Vision-language models.
- multimodal embeddings.
- VLA architectures.
- cross-attention.
- action tokenization/chunking.
- diffusion or flow action heads.
- policy adaptation and fine-tuning.
- Isaac GR00T/other open robot-policy examples.

## Try it

Trace an instruction-to-action pipeline; fine-tune or adapt a feasible pretrained policy; benchmark task success, latency, and out-of-distribution behavior.

Record your setup, inputs, measurements, and failure cases. Keep the experiment small enough to repeat, and compare the result against a simple baseline.

## Further reading

- [LeRobot](https://github.com/huggingface/lerobot)
- [Isaac Lab documentation](https://isaac-sim.github.io/IsaacLab/)

## Next steps

- Apply this topic in the [SO-101 project](../projects/so101.md).
