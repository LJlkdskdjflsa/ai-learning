# ai-learning

A collection of machine learning implementations and experiments using NumPy.

## Contents

- **momentum_rmsprop_numpy_demo.ipynb**: Demonstrates gradient descent optimization algorithms (Vanilla GD, Momentum, RMSprop) using pure NumPy

## Setup

This project uses [`uv`](https://github.com/astral-sh/uv) for fast and reliable Python package management.

### Prerequisites

- Python 3.12 or higher
- uv (install via `curl -LsSf https://astral.sh/uv/install.sh | sh`)

### Installation

```bash
# Create virtual environment and install dependencies
uv sync
```

That's it! `uv` will automatically:
- Create a `.venv` virtual environment
- Install all dependencies from `pyproject.toml`
- Lock versions for reproducibility

### Running Jupyter Notebooks

```bash
# Activate virtual environment
source .venv/bin/activate

# Start Jupyter Notebook
jupyter notebook
```

Or run directly with uv:

```bash
# Run Jupyter without activating the virtual environment
uv run jupyter notebook
```

## Dependencies

- **numpy** `>=1.26.0,<2.0` - NumPy 1.x for compatibility
- **matplotlib** `>=3.10.0` - Plotting and visualization
- **jupyter** `>=1.1.0` - Interactive notebook environment

See [`pyproject.toml`](pyproject.toml) for the complete dependency specification.

## Development

### Adding New Dependencies

```bash
# Add a new package
uv add <package-name>

# Add a development dependency
uv add --dev <package-name>
```

### Updating Dependencies

```bash
# Update all dependencies
uv sync --upgrade
```
