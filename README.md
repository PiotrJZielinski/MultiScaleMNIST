# MultiScaleMNIST dataset

MNIST dataset for detection with multiple scales.

This package creates h5py dataset with images of adjustable size (see config), together
with corner-form bounding boxes `(x0, y0, x1, y1)` and labels.

Examples:

![examples/1.png](examples/1.png) ![examples/2.png](examples/2.png)
![examples/3.png](examples/3.png)

## Development

Requirements:

- Install `pre-commit` (https://pre-commit.com/#install)
- Install `poetry` (https://python-poetry.org/docs/#installation)
- Execute `pre-commit install`
- Use `poetry` to handle requirements
  - Execute `poetry add <package_name>` to add new library
  - Execute `poetry install` to create virtualenv and install packages

## Usage

- Install package with poetry `poetry install`
- Enter the shell `poetry shell`
- Adjust settings by modifying `config.py` or passing config file (see
  `multiscalemnist --help` for info; i.e.
  `multiscalemnist --config-file=config.yml generate`)
- Run generator `multiscalemnist generate`
