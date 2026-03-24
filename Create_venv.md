# How to create the Virtual Environment

## Outline
- 1. Scripts
- 2. What is the scripts means


## 1. Scripts

```
python -m venv .venv
.venv\Scripts\Activate.ps1
```

## 2. What is the scripts means

python -m venv .venv
> python : call python
> -m : call module
> venv : call a module name "venv"
> .venv : create a folder name ".venv" and put the module inside.

.venv\Scripts\Activate.ps1
> call the Activate.ps1 (a powershell file) that place in .venv\Scripts\