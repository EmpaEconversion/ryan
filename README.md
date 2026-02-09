# ryan
Repository to host a pipeline for electrocatalysis CO₂ reduction data analysis and ML

## Windows Setup (PowerShell + uv + Jupyter)

These steps are for **Windows** using **PowerShell**.

1. Install Python, Git, and uv

- Python (Windows download): https://www.python.org/downloads/windows/
- Git (Windows download): https://git-scm.com/download/win
- uv install guide: https://docs.astral.sh/uv/getting-started/installation/

Install `uv` with:

```powershell
pip install uv
```

Close and reopen PowerShell after installing.

2. Move to the folder where you want to keep this repo:

```powershell
cd C:\path\to\your\projects
```

3. Clone the repository:

```powershell
git clone https://github.com/NukP/ryan.git
```

4. Enter the project folder:

```powershell
cd ryan
```

5. Create a virtual environment:

```powershell
uv venv
```

6. Activate the virtual environment:

```powershell
.\.venv\Scripts\activate
```

7. Install dependencies from `pyproject.toml` / `uv.lock`:

```powershell
uv sync
```

8. Register the environment as a Jupyter kernel:

```powershell
python -m ipykernel install --user --name "ryan" --display-name "ryan"
```

9. Select this kernel in VS Code:

- Open a notebook (`.ipynb`).
- In the top-right corner, select **Select Kernel**.
- Choose **Select Another Kernel...**.
- Choose **Jupyter Kernel...**.
- Select **ryan**.

If `ryan` does not appear, refresh the kernel list or restart VS Code.

