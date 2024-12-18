# Python Project with uv

A modern Python project template using uv package manager for fast dependency management.

## Features

- Modern project structure following best practices
- Fast dependency management with uv
- Development tools pre-configured:
  - pytest for testing
  - black for code formatting
  - ruff for linting
  - mypy for type checking

## Getting Started

### Prerequisites

Make sure you have uv installed:

```bash
pip install uv
```

### Setup

1. Clone the repository:
```bash
git clone https://github.com/j0422057/python-uv-project.git
cd python-uv-project
```

2. Create a virtual environment:
```bash
uv venv .venv
source .venv/bin/activate  # On Unix/macOS
# or
.venv\Scripts\activate  # On Windows
```

3. Install dependencies:
```bash
uv pip install -r requirements.txt
uv pip install -r requirements-dev.txt  # for development dependencies
```

### Development

Run tests:
```bash
pytest tests/
```

Format code:
```bash
black src/ tests/
```

Run linter:
```bash
ruff check src/ tests/
```

Run type checker:
```bash
mypy src/
```

## Project Structure

```
my-python-project/
├── .gitignore
├── README.md
├── requirements.txt
├── requirements-dev.txt
├── src/
│   └── my_project/
│       ├── __init__.py
│       └── main.py
└── tests/
    ├── __init__.py
    └── test_main.py
```