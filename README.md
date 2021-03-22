# Example Package
``
pip install --upgrade pip setuptools wheel twine
``
``
python3 -m build
``
``
python3 -m twine upload --repository testpypi dist/*
``

``
pip install -i https://test.pypi.org/simple/ example-pkg-rcsoares
``

``
pip install example-pkg-rcsoares --no-index --find-links file:///./dist
``

#Pull request
https://github.com/xvik/gradle-use-python-plugin/pull/10/commits/9990a7b5e74be90dabd02b7c18ab6da14ceb1732


#Local repository
https://stackoverflow.com/questions/18052217/how-to-create-local-own-pypi-repository-index-without-mirror

# Poetry

poetry is a command-line tool to handle dependency installation and isolation as well as building and packaging of Python packages. It uses pyproject.toml and, instead of depending on the resolver functionality within pip, provides its own dependency resolver. It attempts to speed users’ experience of installation and dependency resolution by locally caching metadata about dependencies.


# Pypiserver

pypiserver is a minimalist application that serves as a private Python package index within organizations, implementing a simple API and browser interface. You can upload private packages using standard upload tools, and users can download and install them with pip, without publishing them publicly. Organizations who use pypiserver usually download packages both from pypiserver and from PyPI.


#JEP

New in version 3.9: You can set the absolute path of the native jep library in code by using MainInterpreter.setJepLibraryPath(String absolutePath);

An example to automatically load the Jep's C library is at https://gist.github.com/vwxyzjn/c054bae6dfa6f80e6c663df70347e238