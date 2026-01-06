# Structural Explainability Organization (.github repo)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![Build Status](https://github.com/structural-explainability/.github/actions/workflows/ci.yml/badge.svg)
[![Check Links](https://github.com/structural-explainability/.github/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/.github/actions/workflows/links.yml)


> GitHub profile repo for the structural-explainability organization on GitHub.


## Developer

Initialize:

```shell
uv self update
uvx pre-commit install
uvx pre-commit run --all-files
```

When starting a new session always git pull:

```shell
git pull
```

Save progress:

```shell
git add -A
# If pre-commit makes changes, re-run `git add -A` before committing.
git commit -m "update"
git push -u origin main
```

## Resources

See `.github\workflows` for available GitHub actions.

See `.devcontainer` for alternatives to local development.
