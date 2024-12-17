# ds-tk-devcontainer

This project provides a development environment for machine learning applications using a Dev Container setup. It is designed to facilitate easy transitions to cloud and production environments while ensuring code quality through automated checks.

## Project Structure

```
ml-dev-container
├── .devcontainer
│   ├── devcontainer.json
│   └── Dockerfile
├── src
│   ├── main.py
│   └── utils
│       └── __init__.py
├── tests
│   ├── test_main.py
│   └── pytest.ini
├── .github
│   └── workflows
│       └── ci.yml
├── .flake8
├── .pre-commit-config.yaml
├── requirements.txt
└── README.md
```

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository:**
   ```
   git clone <repository-url>
   cd ml-dev-container
   ```

2. **Open in VS Code:**
   Open the project in Visual Studio Code and ensure you have the Remote - Containers extension installed.

3. **Reopen in Container:**
   Use the Command Palette (Ctrl+Shift+P) and select "Remote-Containers: Reopen in Container" to build and start the development container.

## Usage

- The main application logic can be found in `src/main.py`.
- Utility functions are located in `src/utils/__init__.py`.
- Unit tests are defined in `tests/test_main.py` and can be run using pytest.

## Code Quality

This project includes several tools to maintain code quality:

- **Flake8**: Style guide enforcement. Configuration is found in `.flake8`.
- **Pre-commit hooks**: Defined in `.pre-commit-config.yaml` to run checks before commits.
- **CI Pipeline**: Continuous integration is configured in `.github/workflows/ci.yml` to automate testing and quality checks.

## Requirements

Dependencies are listed in `requirements.txt`. Install them using:

```
pip install -r requirements.txt
```

## Contributing

Contributions are welcome! Please follow the standard GitHub workflow for submitting issues and pull requests.

## License

This project is licensed under the MIT License. See the LICENSE file for details.