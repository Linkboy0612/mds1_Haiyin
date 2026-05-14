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
