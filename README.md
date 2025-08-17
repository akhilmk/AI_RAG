# Setup Instructions
## 1. Install Python
- Download and install [Anaconda](https://www.anaconda.com/products/distribution).
- Or download and install from the [Python official website](https://www.python.org/downloads/).

## 2. Install VS Code
- Download and install [Visual Studio Code](https://code.visualstudio.com/).

## 3. Install `uv` Package Management  ([uv documentation](https://github.com/astral-sh/uv))
- Windows
  ```sh
  powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex" 
  ```

## 3. Clone the repository:

  ```sh
  git clone https://github.com/<OWNER>/<REPO>.git
  cd <REPO>
  ```
- After checkout, continue with the environment setup steps below.

## 5. Start the Virtual Environment

- This repository already has a UV virtual environment configured, sync it to start:
  ```sh
  uv sync
  ```

- For a fresh Setup (sample commands):
  ```sh
  uv init
  uv venv
  .venv/Scripts/activate
  ```

## 7. Add Packages to Virtual Environment (Optional Sample Commands)
- Add dependencies by command:
  ```sh
  uv add <package-name>
  ```
- Add Jupyter kernel dependencies to `dev` environment:
  ```sh
  uv add ipykernel --dev

## 8. Run File
   Run the Jupyter notebook