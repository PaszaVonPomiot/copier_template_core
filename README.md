# Copier Templates
## Installation

- Install Scoop
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```
- Install pipx
```
scoop install pipx
pipx ensurepath
```

- Restart shell
- Install Copier
```
pipx install copier
```

## Usage
- Create project from template
```
copier copy <template_folder> <destination_folder>

copier copy https://github.com/PaszaVonPomiot/copier_template_core.git project-name

copier copy gh:PaszaVonPomiot/copier_template_core project-name --vcs-ref develop
```

## Templates
https://github.com/PaszaVonPomiot?tab=repositories&q=copier_template

- **Core** - Minimal
    - pyproject.toml
        - Project metadata
        - Development dependencies
        - Mypy settings
        - Ruff settings
    - Git settings
    - PDM settings
    - VSCode & editor settings
    - Pre-commit settings
    - Tests
        - Unit
        - Integration
    - Readme
    - License

- **FastAPI** - Minimal FastAPI with Docker
    - Includes all from Core template
    - FastAPI dependencies
    - Dockerfile
    - Compose file
        - FastAPI service
    - Entrypoint scripts

- **FastAPI_DB** - FastAPI with DB
    - Includes all from FastAPI template
    - Alembic migrations
    - Postgres backend
    - Dockerfile
    - Compose file
        - FastAPI service
        - Postgres service
    - Entrypoint scripts


## Optional
- Configure git aliases on Windows
```
git config --local include.path ../.gitconfig
```

## Template maintenance
- Update pre-commit repos
```
pre-commit autoupdate
```
- Update `.vscode/` extension versions
- Update `pyproject.toml` dependencies versions
- Push new template to git
