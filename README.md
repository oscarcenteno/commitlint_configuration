# commitlint_configuration

This repository is a sample configuration for having a clean git history, using commitlint.
Also, using Github Actions, we test the release preparation process.

In practical terms, every commit is checked locally and in github actions to comply with Conventional Commit Format (https://www.conventionalcommits.org/en/v1.0.0/).

Then, when a pull request is made to "main" branch, a Release PR is created automatically, contaioning an updated CHANGELOG file and bumping the version number according to semver rules.

## setup

- "npm install" will configure commitlint dependencies. There are no other code contents on this repository.

## references

- git repository is configuired following git flow
- git repository is configured with commitlint (https://commitlint.js.org/#/guides-local-setup?id=test)
- Release Please: https://github.com/googleapis/release-please
- Github Action: https://github.com/google-github-actions/release-please-action
