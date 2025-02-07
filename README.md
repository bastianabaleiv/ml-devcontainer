# ds-tk-devcontainer

This project provides a development environment for machine learning applications using Docker based [VSCode Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers). It is designed to facilitate easy transitions to cloud and production environments while ensuring code quality through automated checks.

This project documents my journey through the design decisions made in the following resources, adapting each choice to align with my personal preferences.

- [Microsoft DS Toolkit Dev Containers repository](https://github.com/microsoft/-dstoolkit-devcontainers/) - The original repository that inspired this project. Some key differences include:
  - Ruff usage for style guide enforcement.
  - Docker Compose for easier container management.
  - #todo: GPU support via Docker Compose.
- A Medium article ([The Ultimate VS Code Setup for Python](https://medium.com/ordinaryindustries/the-ultimate-vs-code-setup-for-python-538026b34d94)) that provides a comprehensive guide to setting up a Python development environment in VSCode.

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository:**

```bash
git chttps://github.com/bastianabaleiv/ds-tk-devcontainer.git
cd ds-tk-devcontainer
```

2. **Open in VS Code:**
   Open the project in Visual Studio Code and ensure you have the Remote - Containers extension installed.

3. **Reopen in Container:**
   Use the Command Palette (Ctrl/Cmd+Shift+P) and select "Remote-Containers: Reopen in Container" to build and start the development container.

## Usage

- The main application logic can be coded in `src/main.py`.
- Utility functions can be added at in `src/utils/__init__.py`.
- #todo: ~~Unit tests can be defined in `tests/test_main.py` and can be run using pytest.~~

## Code Quality

This project includes several tools to maintain code quality:

- **ruff**: Style guide enforcement.
- **Pre-commit hooks**: Defined in `.pre-commit-config.yaml` to run checks before commits.
- #todo: ~~**CI Pipeline**: Continuous integration is configured in `.github/workflows/ci.yml` to  automate testing and quality checks.~~

## Requirements

Dependencies are listed in `requirements.txt`. They are installed automatically when the development container is built.

## Contributing

Contributions are not currently accepted. This project is a personal project for learning purposes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
