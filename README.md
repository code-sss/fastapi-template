# FastAPI Template

A template repository for FastAPI projects, ready for VS Code devcontainers, GPU, strict type-checking, linting, and pre-commit hooks.

## Quickstart

```bash
pip install --upgrade pip
pip install -r requirements.txt
uvicorn app.main:app --reload --port 5000
```

Open [http://localhost:5000](http://localhost:5000)

## Development

- Devcontainer: `mcr.microsoft.com/devcontainers/python:1-3.13-bookworm` with GPU support (`--gpus all`)
- VS Code: Preconfigured launch/debug, formatting, linting (see `.vscode/`)
- Pre-commit: ruff, mypy (strict), (see `.pre-commit-config.yaml`)
- Strict type checks: see [`mypy.ini`](./mypy.ini)
- Example code is fully type-annotated for `strict = True`

### Pre-commit hooks

To automatically run the pre-commit on git commit.
```
pre-commit install
```

### Notes

- This template uses mypy's strict mode. All Python functions require type annotations.
- Update the project metadata in `pyproject.toml` as needed.
