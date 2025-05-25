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
# Checking if package is sucessfully installed.
uv pip list
```
