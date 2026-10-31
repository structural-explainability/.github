# Changelog

<!-- markdownlint-disable MD024 -->

All notable changes to this project will be documented in this file.

The format is based on **[Keep a Changelog](https://keepachangelog.com/en/1.1.0/)**
and this project adheres to **[Semantic Versioning](https://semver.org/spec/v2.0.0.html)**.

---

## [Unreleased]

---

## [0.3.0] - 2026-10-31

- Updated after theory updates and older repos are archived.
- 7 original spec- repos archived (e.g. spec-ae)
- 12 original lean repos archived (e.g. AccountableEntities)
- 4 admin repos archived (e.g. se-constitution)

---

## [0.2.0] - 2026-06-04

Released before this changelog existed. See the
[release](https://github.com/structural-explainability/.github/releases/tag/v0.2.0).

---

## [0.1.0] - 2026-06-04

Released before this changelog existed. See the
[release](https://github.com/structural-explainability/.github/releases/tag/v0.1.0).

---

## Notes on versioning and releases

We use SemVer for repository releases:

- **MAJOR** - Breaking changes.
- **MINOR** - Backward-compatible additions.
- **PATCH** - Corrections, documentation, and tooling updates.

Versions are driven by git tags.
Tag `vX.Y.Z` to release.

## Release Procedure (Required)

Follow these steps exactly when creating a new release.

### Task 1. Update release metadata (manual edits)

1.1. CITATION.cff: update version and date-released
1.2. CHANGELOG.md: add section, move unreleased entries, update links
1.3. pyproject.toml: update version

### Task 2. Set up and Validate

```shell
# Update GitHub Actions and pin all action references to immutable SHAs.
uvx gha-tools autoupdate --pin=all --write .github/workflows

# Audit the resulting GitHub configuration for security findings.
uvx zizmor@latest .github/
# some suppressed is still okay

# Validate.
uvx cffconvert --validate
uvx se-manifest-schema validate-manifest --strict

# Format Markdown.
npx markdownlint-cli2 --fix
```

Review all generated and modified files before committing.

### Task 3. Commit and Push

```shell
git add -A
git commit -m "Prep X.Y.Z"
git push -u origin main
```

Verify that all GitHub Actions complete successfully.

### Task 4. Tag and Push the Release

After the required GitHub Actions succeed:

```shell
git tag vX.Y.Z -m "X.Y.Z"
git push origin vX.Y.Z
```

## Only As Needed (delete a tag)

```shell
git tag -d vX.Z.Y
git push origin :refs/tags/vX.Z.Y
```

## Links

[Unreleased]: https://github.com/structural-explainability/.github/compare/v0.3.0...HEAD
[0.3.0]: https://github.com/structural-explainability/.github/releases/tag/v0.3.0
[0.2.0]: https://github.com/structural-explainability/.github/releases/tag/v0.2.0
[0.1.0]: https://github.com/structural-explainability/.github/releases/tag/v0.1.0
