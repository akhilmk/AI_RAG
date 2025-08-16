# Setup Instructions

## 1. Install Anaconda
- Download and install [Anaconda](https://www.anaconda.com/products/distribution).
- Open Anaconda Navigator and check your environment.

## 2. Install VS Code
- Download and install [Visual Studio Code](https://code.visualstudio.com/).

## 3. Create a Python Environment Using `uv` Package Management
- Install `uv` ([uv documentation](https://github.com/astral-sh/uv)):
  ```sh
  pip install uv
  ```

## 4. Create Virtual Environment
- Initialize with `uv`:
  ```sh
  uv init
  ```
## 5. Start the Virtual Environment (Optional)

> Note: The virtual environment is automatically activated when using `uv run`.  
> If you need to manually activate it, use:

- Create the virtual environment:
  ```sh
  uv venv
  ```
- Activate the virtual environment:
  ```sh
  .venv/Scripts/activate
  ```

## 6. Add a `requirements.txt` File (if you want to specify dependencies)
- Place your project dependencies in a `requirements.txt` file to enable easy installation and management.
- Create or add your `requirements.txt` file.

## 7. Add Requirements to Virtual Environment
- Install requirements:
  ```sh
  uv add -r requirements.txt
  ```
- Add dependencies by command:
  ```sh
  uv add <package-name>
  ```
- Add Jupyter kernel dependencies:
  ```sh
  uv add ipykernel

## 8. Run File
   Run the Jupyter notebook