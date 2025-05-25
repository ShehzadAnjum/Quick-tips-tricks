## Creting Project with UV
### Installing UV

## Installation

Install uv with our standalone installers:

```bash
# On macOS and Linux.
curl -LsSf https://astral.sh/uv/install.sh | sh
```

```bash
# On Windows.
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

Or, from [PyPI](https://pypi.org/project/uv/):

```bash
# With pip.
pip install uv
```


```bash
# Adding a package.
uv add <package name>
```

```bash
# The --package flag can be used to create a packaged application:
# i.e. structured as an installable and distributable package.
# It follows a standardized layout (with pyproject.toml, src/, etc.).

uv init --package example-pkg
```


```bash
# Checking if package is sucessfully installed.
uv pip list
```
