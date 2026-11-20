# DSCI522M1
DSCI 522: Milestone 1 project repo

# Project title: Research about the type of iris plant

# Authors : Ramandeep Kaur, Peter Kim, Jiaqi Feng, Carine Ishimwe

(Summary: a short paragraph (view from 10,000 feet) that says what question you asked, what you found at a high level, and 1-2 sentences on what the findings might mean.)
# Summary
We analysis the dataset 'Iris'. Our question is "Which feature (sepal length, sepal width, petal length, petal width) contributes most to predict the type of iris correctly?".

(How to run the analysis: step-by-step instructions that someone who has never seen your project can follow, from cloning the repo to rendering the report. Tell them how to set up the environment (e.g., uv sync) and which command to run. Don’t make the reader guess.)
# How to run the analysis
You could follow the steps to reproduce the analysis.
1. Installation requirements
quarto --version 1.10.18
uv --version 0.12.7
The required Python packages are recorded in `uv.lock`.

2. run the following commands in your Git Bash terminal
cd yourfolder
git clone https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33.git
cd DSCI-522-Group-33
uv sync
uv run quarto render analysis/iris-classification.qmd --to html
analysis/iris-classification.html

(Dependencies: list them (e.g., uv, Quarto) or link to where they are listed (e.g., pyproject.toml).)
# Dependencies
We use uv for dependency management, Quarto for report generation and Python for data analysis.
You can find package requirements in 'pyproject.toml' and `uv.lock`.

(Licenses: the names of the licenses in LICENSE.md (e.g., MIT and CC BY-NC-ND 4.0).)
# Licenses

(AI use statement: say whether you used generative AI (e.g., ChatGPT, Claude, Copilot) in this project. If you did, say how. If you used instruction files (e.g., CLAUDE.md, a system prompt file), commit them to the repo and point to them. Also include a few example prompts.
Link to the rendered report (e.g., your GitHub Pages URL).)
# AI use statement
Using Claude and CHATGPT to debugging code errors and proofreading for grammar and typos before team members review the
code.

# GitHub URL：https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33.git





