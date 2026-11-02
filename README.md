# Physical AI & Embodied Robotics Engineering

> Learning • Simulation • Deployment

![Robotics Engineer](./robotics-engineer.jpg)

An open engineering knowledge hub for building intelligent machines that perceive, learn, reason, plan, and act in the physical world. Explore topic guides, try small experiments, and connect ideas through practical projects.

## Explore

- [Start Here](docs/start-here/index.md) — choose an entry point.
- [Learning Path](LEARNING_PATH.md) — follow a flexible journey through the topics.
- [Foundations](docs/foundations/index.md) — mathematics, programming, perception, and AI.
- [Simulation](docs/simulation/index.md) — kinematics, OpenUSD, physics, and digital twins.
- [Robot Learning](docs/robot-learning/index.md) — demonstrations, reinforcement learning, VLA, and world models.
- [Deployment](docs/deployment/index.md) — hardware, ROS 2, control, inference, and sim-to-real.
- [Projects](docs/projects/index.md) — start with the SO-101 project brief.
- [Resources](docs/resources/index.md) — documentation, research, and community projects.

## Use the learning materials

Read the topic guides directly on GitHub, then follow their prerequisites and suggested experiments. Start with the [PyTorch guide](docs/foundations/pytorch/index.md) if you want to explore tensors, autograd, and training loops. Notebooks live alongside their topic, for example in `docs/foundations/pytorch/notebooks/`.

### 1. Clone the repository

```sh
git clone https://github.com/athivvat/physical-ai-and-embodied-robotics-engineering.git
cd physical-ai-and-embodied-robotics-engineering
```

If you already have the repository, open a terminal in its root directory.

### 2. Create a learning environment

Use Python 3.12 for a new environment. Keep one `.venv` at the repository root so topic notebooks can share it.

On macOS or Linux:

```sh
python3.12 -m venv .venv
source .venv/bin/activate
```

On Windows PowerShell:

```powershell
py -3.12 -m venv .venv
.venv\Scripts\Activate.ps1
```

If you already have a compatible `.venv`, activate it instead of creating another. Check `python --version`; an older environment does not change Python versions when you activate it.

Install the common notebook tools and learning libraries:

```sh
python -m pip install --upgrade pip
python -m pip install -r requirements-notebooks.txt
```

This installs JupyterLab, the Python notebook kernel, NumPy for numerical work, and Matplotlib for plotting. Install additional libraries as you reach topics that need them.

### 3. Install PyTorch

With `.venv` activated, choose the command for your platform:

**macOS:**

```sh
python -m pip install torch torchvision
```

**Linux or Windows, CPU-only:**

```sh
python -m pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu
```

For an NVIDIA or AMD GPU setup, use the [official PyTorch installation selector](https://pytorch.org/get-started/locally/) to choose the supported build for your operating system and compute platform. Run its installation command inside the activated environment. PyTorch is installed separately because its packages depend on your platform.

### 4. Open a notebook

**VS Code:** Install the Python and Jupyter extensions, open the repository folder, and open or create a notebook under `docs/foundations/pytorch/notebooks/`. Click **Select Kernel → Select Another Kernel → Python Environments**, then choose the root `.venv`. Its interpreter is `.venv/bin/python` on macOS/Linux or `.venv\Scripts\python.exe` on Windows. See [VS Code's kernel guide](https://code.visualstudio.com/docs/datascience/jupyter-kernel-management).

**JupyterLab:** From the activated environment at the repository root, run:

```sh
jupyter lab
```

Open the topic's notebook from the file browser, or create a Python notebook there. See the [Jupyter installation guide](https://jupyter.org/install) for other interfaces.

Verify the environment in a notebook cell:

```python
import sys
import torch

print(sys.executable)  # Should point to this repository's .venv
print(torch.__version__)
print(torch.tensor([1.0, 2.0, 3.0]) * 2)
```

Run cells in order, change a small example, and record what you observe. Before sharing results, restart the kernel and run all cells to check that the experiment works from a clean state. Keep dependency versions and setup details with experiments that need to be reproduced.

## Contributing and website development

Share useful resources, reproducible experiments, project results, or corrections. See [CONTRIBUTING.md](CONTRIBUTING.md) for website dependencies, local preview, routes, validation, and GitHub Pages deployment.
