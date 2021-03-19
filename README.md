# Example Package
``
pip install --upgrade pip setuptools wheel twine

python3 -m build

python3 -m twine upload --repository testpypi dist/*
``

``
pip install -i https://test.pypi.org/simple/ example-pkg-rcsoares
``

# Poetry

poetry is a command-line tool to handle dependency installation and isolation as well as building and packaging of Python packages. It uses pyproject.toml and, instead of depending on the resolver functionality within pip, provides its own dependency resolver. It attempts to speed users’ experience of installation and dependency resolution by locally caching metadata about dependencies.


# Pypiserver

pypiserver is a minimalist application that serves as a private Python package index within organizations, implementing a simple API and browser interface. You can upload private packages using standard upload tools, and users can download and install them with pip, without publishing them publicly. Organizations who use pypiserver usually download packages both from pypiserver and from PyPI.
