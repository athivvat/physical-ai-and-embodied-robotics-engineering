# Contributing

Contributions should help readers learn, simulate, or deploy physical AI and embodied robotics systems.

## Add or improve a topic

1. Edit the relevant page under `docs/`, or add a descriptively named Markdown file in the appropriate section.
2. For a new page, add its path to `nav` in `mkdocs.yml`. Navigation paths are relative to `docs/`.
3. Link prerequisites and related topics using relative Markdown paths, such as `../simulation/physics.md`. Avoid domain-root paths because GitHub Pages serves this site under a repository prefix.
4. Cite original documentation or research. Explain what a resource contributes instead of adding an unexplained link.
5. Run `python -m mkdocs build --strict` and resolve warnings before opening a pull request.

Topic guides should include an overview, prerequisites, key concepts, an experiment to try, further reading, and next steps. Keep the emphasis on exploration and engineering practice rather than course IDs or assessments.

## Projects

Distinguish planned experiments from completed work. Record the setup, versions, inputs, baseline, procedure, measured results, and failure cases. Describe hardware testing conditions and operating limits when relevant.

## Images

Place new images in `docs/assets/images/` with descriptive alt text and suitable usage rights. The original `robotics-engineer.jpg` is preserved at the repository root for the README and copied into the website assets; keep those copies identical if updating it.

## Website development setup

Run commands from the repository root. Use Python 3.12, matching the deployment workflow. You can reuse the root `.venv` from the [learning setup](README.md#2-create-a-learning-environment).

If you do not have an environment yet:

```sh
python3.12 -m venv .venv
```

Activate it on macOS/Linux with `source .venv/bin/activate`, or on Windows PowerShell with `.venv\Scripts\Activate.ps1` (create it with `py -3.12 -m venv .venv` on Windows).

Install the website dependencies:

```sh
python -m pip install -r requirements.txt
```

`requirements.txt` contains MkDocs and its theme. `requirements-notebooks.txt` contains optional learning tools; PyTorch is installed separately as described in the README. Website builds do not require PyTorch or execute notebooks.

## Local preview

```sh
python -m mkdocs serve
```

Open the preview address printed by MkDocs. The project URL prefix is included in the preview path. Saved edits reload the preview; stop the server with Ctrl+C.

## Build and validate

```sh
python -m mkdocs build --strict
git diff --check
```

Resolve broken internal links and anchors before submitting a pull request. Generated files go into `site/`, which is excluded from Git. Keep `.venv/` and generated output out of commits.

## Structure and routes


- `docs/` holds the authoritative website content.
- `docs/index.md` is the homepage.
- `docs/robot-learning/world-models.md` becomes `/robot-learning/world-models/` under the site's project URL.
- `mkdocs.yml` controls navigation, theme, search, and link validation.
- `LEARNING_PATH.md` links to the suggested journey, replacing the former course syllabus.

Use descriptive filenames and relative Markdown links. Keep topic details in `docs/` so the README and learning-path entry point stay concise.

Group a topic's guide and notebooks together, for example:

```text
docs/foundations/pytorch/
├── index.md
└── notebooks/
    └── your-experiment.ipynb
```

`docs/foundations/pytorch/index.md` maps to `/foundations/pytorch/`. Link to Markdown sources, such as `pytorch/index.md`, rather than hard-coding generated HTML URLs.

The current website build does not render `.ipynb` files as notebook pages. Keep notebook files valid and usable in Jupyter or VS Code; adding notebook rendering requires a MkDocs notebook plugin and corresponding navigation entries.

## Publish on GitHub Pages


1. In the GitHub repository, open **Settings → Pages**.
2. Set **Build and deployment → Source** to **GitHub Actions**.
3. Push these files to `main`, or run **Build and deploy documentation** from the Actions tab after the workflow is on GitHub.

The workflow validates pull requests and publishes successful builds from `main`. Once deployed, the site will be available at:

https://athivvat.github.io/physical-ai-and-embodied-robotics-engineering/

The workflow uses GitHub's built-in token; no personal access token or custom domain is needed. If you fork the repository, update `site_url` and `repo_url` in `mkdocs.yml` before publishing.
