# How to create the Virtual Environment

## Outline
- 0. Install Python (Windows 11)
- 1. Scripts
- 2. Install packages in the virtual environment
- 3. What is the scripts means


## 0. Install Python (Windows 11)

### Step 1 — Download Python
Go to https://www.python.org/downloads/ and download the latest version for Windows.

### Step 2 — Install Python
Run the installer.
> **Important:** Check the box **"Add python.exe to PATH"** before clicking Install Now.

### Step 3 — Verify installation
Open PowerShell and run:
```
python --version
pip --version
```
You should see both versions printed. If yes, Python and pip are ready.

### Step 4 — Allow script execution (PowerShell only)
Run this once to allow virtual environment activation:
```
Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
```


## 1. Scripts

Note: for Windows 11 (PowerShell)
```
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Note: for Windows 11 (CMD)
```
python -m venv .venv
.venv\Scripts\activate.bat
```

## 2. Install packages in the virtual environment

> Make sure the virtual environment is activated first (you should see `(.venv)` in your terminal).

Install a single package:
```
pip install <package-name>
```

Install multiple packages at once:
```
pip install <package1> <package2>
```

Install from a requirements file:
```
pip install -r requirements.txt
```

Check installed packages:
```
pip list
```

Save current packages to a requirements file:
```
pip freeze > requirements.txt
```


## 3. What is the scripts means

python -m venv .venv
> python : call python
> -m : call module
> venv : call a module name "venv"
> .venv : create a folder name ".venv" and put the module inside.

.venv\Scripts\Activate.ps1
> call the Activate.ps1 (a powershell file) that place in .venv\Scripts\
