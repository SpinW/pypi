# PyPi Repo
Simple slimline repo acting as a PyPi server for spinw packages. 

See [https://spinw.org/pypi/](https://spinw.org/pypi/)

# Using with pip
Simply install with the modified call:
```
pip install -v spinw --extra-index-url https://spinw.org/pypi/
```

# Using pyproject.toml 
Add the following to your `pyproject.toml`:
```
[[tool.poetry.source]]
name = "spinWsource"
url = "https://spinw.org/pypi/"
secondary = true
```
Dependencies can then be added the usual way
