# Python Project with GitHub Codespaces

Welcome to this simple project designed to explore **GitHub Codespaces** and Python programming. This repository contains a basic Python script that calculates the sum of a list of numbers, perfect for getting started with Codespaces.

## Prerequisites

- A GitHub account with access to [GitHub Codespaces](https://github.com/codespaces).
- No local software installation is required, as Codespaces provides a cloud-based environment with Python pre-installed.

## Project Contents

- `somme.py`: A Python script that defines a function to calculate the sum of a list of numbers.
- `.devcontainer/devcontainer.json`: (Optional) Configuration file to customize the Codespaces environment.
- `requirements.txt`: List of Python dependencies (e.g., `numpy`).

## Getting Started

1. **Create a Codespace**:
   - Open this repository on GitHub.
   - Click **Code** > **Codespaces** > **Create codespace on main**.
   - Wait for the environment to load in your browser or VS Code.

2. **Run the Script**:
   - Open the `somme.py` file.
   - In the terminal (accessible via `Ctrl + ~`), run:
     ```bash
     python somme.py
     ```
   - The output will display the sum of a list of numbers (e.g., `[1, 2, 3, 4, 5]`).

3. **Install Dependencies** (if needed):
   - To use `numpy` (optional), run:
     ```bash
     pip install -r requirements.txt
     ```
   - Modify `somme.py` to test with `numpy` if desired.

4. **Manage Versions with Git**:
   - Check changes:
     ```bash
     git status
     ```
   - Stage files:
     ```bash
     git add .
     ```
   - Commit changes:
     ```bash
     git commit -m "Add somme.py script"
     ```
   - Push to GitHub:
     ```bash
     git push origin main
     ```

## Repository Structure

```
├── somme.py                # Main Python script
├── requirements.txt        # Python dependencies
├── .devcontainer/          # Codespaces configuration (optional)
│   └── devcontainer.json
└── README.md               # This file
```

## Customize the Environment

To add libraries or configure the environment, edit `.devcontainer/devcontainer.json`. Example to include `numpy` and the Python extension for VS Code:

```json
{
  "name": "Python Simple",
  "image": "mcr.microsoft.com/devcontainers/python:3.9",
  "postCreateCommand": "pip install -r requirements.txt",
  "customizations": {
    "vscode": {
      "extensions": ["ms-python.python"]
    }
  }
}
```

## Best Practices

- **Save Regularly**: Commit and push changes with Git to avoid losing work.
- **Test Your Code**: Add test cases in `somme.py` (e.g., empty list or negative numbers).
- **Document**: Use comments and docstrings to make your code clear.
- **Stop the Codespace**: If unused, stop it via the GitHub interface to save resources.

## Useful Resources

- [GitHub Codespaces Documentation](https://docs.github.com/en/codespaces): Guide to setting up and managing Codespaces.

---

This project is a starting point for exploring Codespaces. Feel free to clone, modify, and share your own scripts!
