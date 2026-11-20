# Contributing to the Iris Species Classification Project

Thanks for your interest in contributing! This project is maintained by DSCI 522 Group 33 (UBC Master of Data Science). We welcome contributions from team members and the wider community.

Everyone participating in this project is expected to follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Ways to contribute

- **Report a bug or problem:** open an [issue](https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33/issues) and include:
  - what you expected to happen and what actually happened,
  - the steps to reproduce the problem (which file or code chunk, and what you ran),
  - any error message or traceback, pasted as text, and
  - your operating system and Python version.
- **Suggest an improvement:** open an [issue](https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33/issues) describing the change and why it would help. Please discuss the idea there before starting work on it.
- **Fix something or add a feature:** follow the workflow below.

Before opening a new issue, please search the existing [issues](https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33/issues) and [pull requests](https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33/pulls) to check whether it has already been raised.

## Development workflow

1. **Set up the environment.** This project uses [uv](https://docs.astral.sh/uv/) to manage Python (version 3.14, pinned in `.python-version`) and its packages (listed in `pyproject.toml` and locked in `uv.lock`). The report is written in [Quarto](https://quarto.org/docs/get-started/), which you need to install separately. After installing uv and Quarto, run from the root of the repository:

   ```bash
   uv sync
   ```

   This creates a `.venv/` folder with the exact package versions in `uv.lock`.

2. **Create a branch** off an up-to-date `main` with a short, descriptive name:

   ```bash
   git switch main
   git pull
   git switch -c fix-eda-plot
   ```

3. **Make your changes** in small, focused commits with clear messages (for example, `Add confusion matrix to analysis report`). The Quarto report (`.qmd`) goes in `analysis/`; raw data goes in `data/raw/` and processed data in `data/processed/`.

4. **Check your work** by rendering the report inside the project environment, to make sure it still runs end to end without errors:

   ```bash
   uv run quarto render analysis/
   ```

5. **Push and open a pull request** into `main`:

   ```bash
   git push -u origin fix-eda-plot
   ```

   In the pull request description, explain what you changed and why, link any related issue (for example, `Closes #12`), and include an AI disclosure if one is needed (see the [AI policy](#ai-policy)).

6. **Code review:** at least one other team member must review and approve the pull request before it is merged. Reviewers should leave constructive, specific feedback. Authors respond by pushing new commits to the same branch.

## Team norms

- Do not push directly to `main`; all changes go through pull requests.
- Keep pull requests small enough to review in one sitting.
- Do not commit the `.venv/` folder, Quarto's `.quarto/` cache, `.ipynb_checkpoints/`, or other generated files; see `.gitignore`.
- If you need a new package, add it with `uv add <package-name>`. This updates both `pyproject.toml` and `uv.lock`; commit both files in the same pull request as the code that uses the package.

## AI policy

You may use generative AI tools (for example, ChatGPT, GitHub Copilot, or Claude) to help you contribute to this project, such as to explain errors, brainstorm, draft code, or improve wording, under the following rules.

- **People, not AI agents, run the repository.** Issues and pull requests must be opened, reviewed, and merged by a human contributor. AI agents or bots must not open, review, or merge them on anyone's behalf, and review comments must reflect your own judgement.
- **Disclose substantial AI use.** If an AI tool generated a substantial part of your contribution (code, analysis, or text), say so in the pull request description: name the tool and briefly describe what it was used for and which files it affected. Minor uses, such as single-line autocomplete or spell-checking, do not need to be disclosed.
- **You are responsible for what you submit.** You must read, run, and understand everything in your contribution, whether or not an AI tool helped write it, and be able to explain it during review. You are also responsible for making sure it is correct and does not copy anyone else's work without proper attribution.

Reviewers may ask contributors to explain, revise, or remove AI-generated content.

## Attribution

These guidelines were adapted from the contributing guidelines of the [UBC-MDS breast cancer predictor](https://github.com/ttimbers/breast_cancer_predictor_py/blob/main/CONTRIBUTING.md) example project, which is itself based on the [dplyr contributing guide](https://github.com/tidyverse/dplyr/blob/main/.github/CONTRIBUTING.md). The AI policy was adapted from the [SymPy AI-generated code policy](https://docs.sympy.org/dev/contributing/ai-generated-code-policy.html) and the [earthaccess AI policy](https://earthaccess.readthedocs.io/en/latest/contributor/ai-policy/).
