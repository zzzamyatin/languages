# Articles
* https://cjolowicz.github.io/posts/hypermodern-python-01-setup/
* https://venthur.de/2021-06-26-python-packaging.html


# dependency management
pipenv  # recommended by PyPA, but suxx
poetry  # cool

# distributions
PyPI / pip
Anaconda / conda

# setup
setup.py + requirements.txt  # currently best, others suxx

setup.cfg
pipfile + pipfile.lock
pyproject.toml



# what are we using now?
```
where python # executable location in win
which python # executable location in macos and unix
python --version
python3
py
py3
```

# freeze
conda env export > environment.yml

`conda env export` has problems:
* different on macOS and Win
* channels in random order
* smth else
Script [`conda-lock`](https://github.com/conda-incubator/conda-lock/) solves them.

# create an environment
`python -m venv ...`
`conda env create -n envname -f environment.yml`

# activate an environment
```
conda activate
```

## check success
```
where python # executable location in win
which python # executable location in macos and unix
python --version
```

# install a package
`pip install`
`conda install`


# package code
* as a zip file https://docs.python.org/3/library/zipapp.html
