# DSCI522M1
DSCI 522: Milestone 1 project repo

# Project title: Research about the type of iris plant

# Authors
Ramandeep Kaur, Peter Kim, Jiaqi Feng, Carine Ishimwe

# Summary
We analysis the dataset 'Iris'. Our question is "Which feature (sepal length, sepal width, petal length, petal width) contributes most to predict the type of iris correctly?"....

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


# Dependencies
We use uv for dependency management, Quarto for report generation and Python for data analysis.
You can find package requirements in 'pyproject.toml' and `uv.lock`.


# Licenses


# AI use statement
Using Claude and CHATGPT to debugging code errors and proofreading for grammar and typos before team members review the
code.

# GitHub URL
https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33.git





