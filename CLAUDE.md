# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build/Run Commands
- Install dependencies: `npm i -d` and `pipenv sync`
- Build frontend: `npx webpack`
- Run locally: `docker compose -f deploy/localdev/docker-compose.yml up --build`
- Run tests: `pipenv run pytest`
- Run single test: `pipenv run pytest tests/path/to/test_file.py::test_name -v`
- Run JS tests: `npm test`

## Code Style Guidelines
- Python: Follow PEP 8 style guidelines
- JavaScript: Use modern ES6+ features and syntax
- Imports: Group standard library, third-party, and local imports
- Error handling: Use explicit error handling and logging
- Types: Use type annotations in Python functions
- Naming conventions:
  - Python: snake_case for variables/functions, PascalCase for classes
  - JavaScript: camelCase for variables/functions, PascalCase for classes
- Tests: Mark tests with appropriate categories (e.g. @pytest.mark.quick)
- Docker: Multiple services coordinate via Docker Compose