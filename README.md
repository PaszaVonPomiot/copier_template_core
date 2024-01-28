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
```
copier copy <template_folder> <destination_folder>
```


## Templates

https://github.com/PaszaVonPomiot?tab=repositories&q=copier_template

- **Core** - Minimal
    - pyproject.toml
        - Project metadata
        - Development dependencies
        - Black settings
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


