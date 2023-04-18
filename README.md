# Versioning and Release management tools (JS)

## Home work: Base app with commint lint + release-please

This repository is a sample configuration for having a clean git history, using commitlint.
Also, using Github Actions, we test the release preparation process.

In practical terms, every commit is checked locally and in github actions to comply with Conventional Commit Format (https://www.conventionalcommits.org/en/v1.0.0/).

Then, when a pull request is made to "main" branch, a Release PR is created automatically, contaioning an updated CHANGELOG file and bumping the version number according to semver rules.

## home task

Task is specified in home_task/"Release and versioning automation tools - home task.pdf"

Note that standard-version is not used as it is deprecated as of today (2023.04.18), so I used release-please as it offers integration with CI pipeline.

## setup

- "npm install" will configure commitlint dependencies. There are no other code contents on this repository.

## references

- git repository is configured following git flow
- git repository is configured with commitlint (https://commitlint.js.org/#/guides-local-setup?id=test)
- Release preparation is done with "Release Please": https://github.com/googleapis/release-please
- Github Action: https://github.com/google-github-actions/release-please-action
