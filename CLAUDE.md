# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Python project following along with the "Neural Networks: Zero to Hero" tutorial series. The project implements neural network components from scratch, focusing on building a micrograd-style automatic differentiation library.

## Development Environment

- **Package Manager**: Uses `uv` (ultra-fast Python package manager)
- **Python Version**: Requires Python >=3.10, currently using 3.11.13
- **Main Dependencies**: matplotlib, numpy
- **Dev Dependencies**: ipykernel, jupyterlab

## Common Commands

### Environment Setup
```bash
# Install dependencies
uv sync

# Add a new dependency
uv add <package-name>

# Add a dev dependency
uv add --dev <package-name>
```

### Running Code
```bash
# Run the main script
uv run main.py

# Run Python with project dependencies
uv run python

# Start Jupyter Lab for notebook work
uv run jupyter lab
```

### Development
```bash
# Update dependencies
uv lock

# Export requirements (if needed)
uv export > requirements.txt
```

## Project Structure

- `micrograd_from_scratch_yay.ipynb`: Jupyter notebook containing the main implementation work
- `pyproject.toml`: Project configuration and dependencies
- `uv.lock`: Locked dependency versions
- `main.py`: Entry point with basic hello world functionality, placeholder for now.

## Architecture Notes

The project is centered around implementing neural network fundamentals in a Jupyter notebook environment. The main development workflow involves:

1. Implementing concepts in the notebook with visualization using matplotlib
2. Using numpy for numerical operations
3. Building from first principles without high-level ML frameworks

The notebook-first approach allows for interactive development and visualization of neural network concepts as they're implemented.
