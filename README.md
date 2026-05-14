# Python Development Setup with GitHub Codespaces and VS Code

## Introduction

This guide will help you to set up a professional Python development environment using:

- GitHub
- GitHub Codespaces
- VS Code Desktop
- Python Virtual Environments
- Jupyter Notebook
- Git Version Control

By the end of this tutorial, you will be able to:

✅ Create a GitHub repository  
✅ Launch a GitHub Codespace  
✅ Connect Codespaces to VS Code Desktop  
✅ Create and manage a Python project  
✅ Set up virtual environments  
✅ Configure Python interpreters  
✅ Install Jupyter Notebook and libraries  
✅ Save and push code to GitHub  

---

# Step 1 — Create a GitHub Repository

1. Go to:

```text
https://github.com
```

2. Sign in to your GitHub account

3. Click the **+** icon in the top-right corner

4. Select:

```text
New repository
```

5. Enter a repository name

Example:

```text
python-learning-project
```

6. Add a short description

7. Select:

- Public OR Private

8. Check:

```text
Add a README file
```

9. Click:

```text
Create repository
```

---

# Step 2 — Start GitHub Codespaces

1. Open your repository

2. Click the green:

```text
Code
```

button

3. Select the:

```text
Codespaces
```

tab

4. Click:

```text
Create codespace on main
```

Wait a few moments while GitHub prepares your cloud development environment.

---

# Step 3 — Connect Codespaces to VS Code Desktop

## Install VS Code

Download and install VS Code:

```text
https://code.visualstudio.com/
```

---

## Install Required Extensions

Open VS Code and install:

### Python Extension

```text
Python
```

### Jupyter Extension

```text
Jupyter
```

### GitHub Codespaces Extension

```text
GitHub Codespaces
```

---

## Connect to Codespace

1. Open VS Code

2. Press:

### Windows/Linux

```text
Ctrl + Shift + P
```

### macOS

```text
Cmd + Shift + P
```

3. Search for:

```text
Codespaces: Connect to Codespace
```

4. Select your Codespace

Now your cloud environment is connected to VS Code Desktop.

---

# Step 4 — Create Your Project Folder

Open the terminal inside VS Code and run:

```bash
mkdir my_project
cd my_project
```

Example:

```bash
mkdir data_analysis_project
cd data_analysis_project
```

---

# Step 5 — Check Python Version

Run:

```bash
python --version
```

or:

```bash
python3 --version
```

Example output:

```text
Python 3.12.1
```

---

# Step 6 — Create a Virtual Environment

Create a virtual environment named `.venv`:

```bash
python -m venv .venv
```

If needed:

```bash
python3 -m venv .venv
```

---

# Step 7 — Activate the Virtual Environment

## Linux / macOS / Codespaces

```bash
source .venv/bin/activate
```

## Windows PowerShell

```powershell
.venv\Scripts\Activate.ps1
```

After activation, your terminal should display:

```text
(.venv)
```

---

# Step 8 — Select Python Interpreter in VS Code

1. Press:

```text
Ctrl + Shift + P
```

2. Search:

```text
Python: Select Interpreter
```

3. Choose the interpreter from:

```text
.venv
```

---

# Step 9 — Upgrade pip

Run:

```bash
python -m pip install --upgrade pip
```

---

# Step 10 — Install Jupyter Notebook

Install Jupyter support:

```bash
pip install notebook jupyter ipykernel
```

Register the environment as a Jupyter kernel:

```bash
python -m ipykernel install --user --name=my_project_env --display-name "Python (my_project_env)"
```

---

# Step 11 — Install Common Python Libraries

Install useful libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

Optional libraries:

```bash
pip install requests beautifulsoup4 plotly openpyxl
```

---

# Step 12 — Save Project Dependencies

Create a `requirements.txt` file:

```bash
pip freeze > requirements.txt
```

To install later:

```bash
pip install -r requirements.txt
```

---

# Step 13 — Create Your First Python File

Create:

```text
main.py
```

Add:

```python
print("Hello World!")
```

Run:

```bash
python main.py
```

---

# Step 14 — Create a Jupyter Notebook

Create a notebook file:

```text
notebook.ipynb
```

Select the kernel:

```text
Python (my_project_env)
```

Test the notebook:

```python
import pandas as pd
import numpy as np

print("Notebook is ready!")
```

---

# Step 15 — Recommended Project Structure

```text
python-learning-project/
│
├── README.md
├── requirements.txt
├── .gitignore
│
└── my_project/
    ├── main.py
    ├── notebook.ipynb
    └── .venv/
```

---

# Step 16 — Create a `.gitignore` File

Create:

```text
.gitignore
```

Add:

```gitignore
.venv/
__pycache__/
.ipynb_checkpoints/
*.pyc
.env
```

This prevents unnecessary files from being uploaded to GitHub.

---

# Step 17 — Check Git Status

Run:

```bash
git status
```

---

# Step 18 — Add Files to Git

Run:

```bash
git add .
```

---

# Step 19 — Commit Changes

Run:

```bash
git commit -m "Initial project setup"
```

---

# Step 20 — Push Changes to GitHub

Run:

```bash
git push
```

Your project is now saved to GitHub.

---

# Daily Development Workflow

Each time you work on your project:

```bash
git status
git add .
git commit -m "Describe your changes"
git push
```

Example:

```bash
git add .
git commit -m "Add data visualization notebook"
git push
```

---

# Final Checklist

Before submission, make sure you have completed:

- [ ] Created a GitHub repository
- [ ] Started a GitHub Codespace
- [ ] Connected Codespaces to VS Code
- [ ] Created a project folder
- [ ] Created a virtual environment
- [ ] Activated the virtual environment
- [ ] Selected the Python interpreter
- [ ] Installed Jupyter Notebook
- [ ] Installed required libraries
- [ ] Created `requirements.txt`
- [ ] Created `.gitignore`
- [ ] Created Python files or notebooks
- [ ] Committed changes
- [ ] Pushed changes to GitHub

---


