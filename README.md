# DSCI522M1
DSCI 522: Milestone 1 project repo

# Project title: Research about the type of iris plant

# Authors
Ramandeep Kaur, Peter Kim, Jiaqi Feng, Carine Ishimwe

# Summary
We analysis the dataset 'Iris'. Our question is "Which feature (sepal length, sepal width, petal length, petal width) contributes most to predict the type of iris correctly?"....

# How to run the analysis
You could follow the steps to reproduce the analysis.
- Installation requirements
1. quarto --version 1.10.18
2. uv --version 0.12.7
3. The required Python packages are recorded in `uv.lock`.

- run the following commands in your Git Bash terminal
1. cd yourfolder
2. git clone https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33.git
3. cd DSCI-522-Group-33
4. uv sync
5. uv run quarto render analysis/iris-classification.qmd --to html
6. analysis/iris-classification.html


# Dependencies
We use uv for dependency management, Quarto for report generation and Python for data analysis.
You can find package requirements in 'pyproject.toml' and `uv.lock`.


# Licenses


# AI use statement
Using Claude and CHATGPT to debugging code errors and proofreading for grammar and typos before team members review the
code.

# GitHub URL
https://github.com/UBC-MDS-2026-27/DSCI-522-Group-33.git





