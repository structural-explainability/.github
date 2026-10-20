# Structural Explainability Organization (.github repo)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/license/MIT)
![Build Status](https://github.com/structural-explainability/.github/actions/workflows/ci-hygiene.yml/badge.svg?branch=main)
[![Check Links](https://github.com/structural-explainability/.github/actions/workflows/links.yml/badge.svg)](https://github.com/structural-explainability/.github/actions/workflows/links.yml)

> GitHub profile repo for the structural-explainability organization on GitHub.

## Developer Command Reference

<details>
<summary>Show command reference</summary>

### Install Tools

This repository is not a Python package and does not require a local virtual
environment.
It does use Python-based command-line tools through `uvx`,
and it uses Node.js for Markdown linting through `npx`.
Install these tools once on your machine:

- `uv`
- Node.js / npm
- Git

### In a machine terminal

Open a machine terminal where you want the project:

```shell
git clone https://github.com/structural-explainability/se-codeowners

cd se-codeowners
code .
```

### In a VS Code terminal

Use VS Code Menu:
View / Command Palette / `Developer: Reload Window` to refresh.

```shell
uv self update
uvx prek install --force
uvx prek update

# Update GitHub Actions and pin all action references to immutable SHAs.
uvx gha-tools autoupdate --pin=all --write .github/workflows

# Audit the resulting GitHub configuration for security findings.
# NO .github\workflows\deploy-zensical.yml
uvx zizmor@latest .github/

# Validate.
uvx cffconvert --validate
uvx se-manifest-schema validate-manifest --strict

# lint and validate files
npx markdownlint-cli2 --fix
uvx se-manifest-schema validate-manifest --strict
uvx cffconvert --validate

# generate and check CODEOWNERS
uvx se-codeowners generate --strict --output .github/CODEOWNERS
uvx se-codeowners check

 # save changes
git add -A
uvx prek run --all-files
# repeat if changes were made
git add -A
uvx prek run --all-files

# save progress
git add -A
git commit -m "update"
git push -u origin main

# tag as needed (to match CITATION.cff)
git tag vX.Y.Z -m "X.Y.Z"
git push origin vX.Y.Z
```

## Authority Manifest

[.accountability/surfaces.toml](./.accountability/surfaces.toml)

## Citation

[CITATION.cff](./CITATION.cff)

## License

[MIT](./LICENSE)

## Repository Manifest

[SE_MANIFEST.toml](./SE_MANIFEST.toml)
