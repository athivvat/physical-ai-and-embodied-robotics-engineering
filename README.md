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

## Local preview

Requires Python 3.10 or later. The deployment workflow uses Python 3.12.

```sh
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
python -m mkdocs serve
```

Open the preview address printed by MkDocs. The project URL prefix is included in the preview path.

Build and validate the site before submitting changes:

```sh
python -m mkdocs build --strict
```

Generated files go into `site/`, which is excluded from Git.

## Publish on GitHub Pages

1. In the GitHub repository, open **Settings → Pages**.
2. Set **Build and deployment → Source** to **GitHub Actions**.
3. Push these files to `main`, or run **Build and deploy documentation** from the Actions tab after the workflow is on GitHub.

The workflow validates pull requests and publishes successful builds from `main`. Once deployed, the site will be available at:

https://athivvat.github.io/physical-ai-and-embodied-robotics-engineering/

The workflow uses GitHub's built-in token; no personal access token or custom domain is needed. If you fork the repository, update `site_url` and `repo_url` in `mkdocs.yml` before publishing.

## Structure and routes

- `docs/` holds the authoritative website content.
- `docs/index.md` is the homepage.
- `docs/robot-learning/world-models.md` becomes `/robot-learning/world-models/` under the site's project URL.
- `mkdocs.yml` controls navigation, theme, search, and link validation.
- `contents/` retains links from the original resource collection to the new pages.
- `LEARNING_PATH.md` links to the suggested journey, replacing the former course syllabus.

Use descriptive filenames and relative Markdown links. Keep topic details in `docs/` so the README and learning-path entry point stay concise.

## Contributing

Share useful resources, reproducible experiments, project results, or corrections. See [CONTRIBUTING.md](CONTRIBUTING.md) for authoring and validation guidance.
