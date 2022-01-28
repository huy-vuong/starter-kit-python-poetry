![GitHub Actions Build Status](https://github.com/yanz777/react-blank-project/actions/workflows/build.yml/badge.svg)

# starter-kit-python-poetry
For starting new Python projects managed in Poetry

## Getting Started

### Running the Project

In `pyproject.toml`, there's a header `[tool.poetry.scripts]`, which allows for the user to run scripts via `poetry run ${script_name}`.

For this project, the entry point is in `starter_kit/starter_kit.py` in the `main` function, so to set this up, the `pyproject.toml` looks like this:

```toml
[tool.poetry.scripts]
starter_kit = "starter_kit.starter_kit:main"
```

This means that running `poetry run starter_kit` would look in the `starter_kit/` directory for an `starter_kit.py` and run the `main` function inside it. For this repo, `poetry run starter_kit` would print `Hello world!` to the console and exit.
