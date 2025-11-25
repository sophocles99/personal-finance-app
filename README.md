# Personal Finance App
Welcome to the beautifully-named **Personal Finance App**. This app allows users to manage their personal finances by keeping track of income and expenses, making budgets, and using many more exiting features that we haven't decided on yet.

## Tech Stack
- Database - PostgreSQL
- Backend - Django
- Frontend - React Native

## Getting Started - Backend
We use Python 3.14 for this project. The recommended tool for managing Python versions and virtual environments is [uv](https://docs.astral.sh/uv/).

### Install uv
If you're using a Mac, the easiest way to install uv is using homebrew:
```bash
brew install uv
```
Otherwise, follow the [installation guide](https://docs.astral.sh/uv/getting-started/installation/). (It's fine to install uv globally.)

### Install project dependencies
From the project root, type:
```bash
cd backend
uv sync
```
The `uv sync` command checks `uv.lock` to make sure that exactly the right versions of the project dependencies are installed.

It also reads the `.python-version` files and creates a virtual environment in the default folder `.venv`. The virtual environment contains the specific version of Python needed, and the project dependencies. It keeps them separate from anything that is installed globally, preventing clashes and confusion. (uv automatically downloads the required version of Python if you don't have it.)

### Activate the virtual environment
```bash
source .venv/bin/activate
```

### Run the project
```bash
python main.py
```