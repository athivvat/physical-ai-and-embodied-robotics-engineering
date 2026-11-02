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

## Preview and deployment

Follow the local preview instructions in [README.md](README.md). Pull requests build the site without publishing it; updates to `main` deploy through GitHub Actions once Pages is enabled.
