# Copier Templates

## Installation
- Update pip - `python.exe -m pip install --upgrade pip`
- Install pipx - `pip install --user pipx`
- Update PATH - `.\pipx.exe ensurepath`
- Restart shell
- Install Copier - `pipx install copier`



## Templates
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
    
# Docs
https://copier.readthedocs.io/en/stable/
