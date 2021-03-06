# Implementing the Clean Architecture - Auctions
Example app.

[![Build Status](https://travis-ci.org/Enforcer/clean-architecture.svg?branch=master)](https://travis-ci.org/Enforcer/clean-architecture)

# Work with the repo
Pycharm - mark each package as Sources Root.
![Marking directories as source root in PyCharm](docs/marking_as_sources_root.png)
Console - `make dev` to install each subpackage in editable mode.

# Work with docker containers
```bash
# Start everything
docker-compose up --build

# Black formatting
docker-compose exec -T app black -l 120 ./
# isort
docker-compose exec -T app isort --recursive ./
# flake8 checks
docker-compose exec -T app flake8 --max-line-length 120 ./
```


