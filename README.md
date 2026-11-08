# Calculator CI Project

A simple Python calculator with automated unit tests using Pytest and a GitHub Actions CI pipeline.

## Project structure

```text
calculator-ci-project/
├── calculator.py
├── test_calculator.py
├── requirements.txt
├── .gitignore
├── README.md
└── .github/
    └── workflows/
        └── ci.yml
```

## Run locally in VS Code

1. Open this folder in VS Code.
2. Open Terminal → New Terminal.
3. (Optional) Create and activate a virtual environment:

   Windows PowerShell:
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

   If PowerShell blocks activation, use Command Prompt:
   ```cmd
   .venv\Scripts\activate.bat
   ```

4. Install dependencies:
   ```bash
   python -m pip install -r requirements.txt
   ```

5. Run the tests:
   ```bash
   python -m pytest -v
   ```

Expected result: `5 passed`.

## Run the GitHub Actions CI pipeline

1. Create a new empty GitHub repository named `calculator-ci-project`.
2. In this project folder's terminal, run:

   ```bash
   git init
   git branch -M main
   git add .
   git commit -m "Add calculator CI project"
   git remote add origin https://github.com/YOUR_USERNAME/calculator-ci-project.git
   git push -u origin main
   ```

3. Replace `YOUR_USERNAME` with your GitHub username.
4. Open your GitHub repository and select the **Actions** tab.
5. Open **Calculator CI Pipeline** to see the automatic test run.

The workflow runs on pushes and pull requests targeting the `main` branch.
