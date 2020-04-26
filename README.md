# Python Best Practices Cookiecutter

Best practices [cookiecutter](https://github.com/audreyr/cookiecutter) template as described in this [blogpost](https://sourcery.ai/blog/python-best-practices/).

## Features
- Testing with [pytest](https://docs.pytest.org/en/latest/)
- Formatting with [black](https://github.com/psf/black)
- Import sorting with [isort](https://github.com/timothycrosley/isort)
- Linting with [flake8](http://flake8.pycqa.org/en/latest/)
- Git hooks that run all the above with [pre-commit](https://pre-commit.com/)

## Quickstart
```sh
# Install Poetry
curl -sSL https://raw.githubusercontent.com/sdispater/poetry/master/get-poetry.py | python

# Install cookiecuuter
brew install python3
# or "pip install --user cookiecutter"

# Use cookiecutter to create project from this template
cookiecutter gh:MattiooFR/python-best-practices-cookiecutter # gh: is abbreviation for github path

# Enter project directory
cd <repo_name>

# Initialise git repo
git init

# Install dependencies
poetry install

# Setup pre-commit and pre-push hooks
poetry run pre-commit install -t pre-commit
poetry run pre-commit install -t pre-push
```
