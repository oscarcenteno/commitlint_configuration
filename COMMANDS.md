# COMMANDS

Followed from https://github.com/conventional-changelog/commitlint

## Install commitlint cli and conventional config

npm install --save-dev @commitlint/config-conventional @commitlint/cli

## Configure commitlint to use conventional config

echo "module.exports = {extends: ['@commitlint/config-conventional']}" > commitlint.config.js

## To lint commits before they are created you can use Husky's commit-msg hook:

npm install husky --save-dev

npx husky install

npx husky add .husky/commit-msg 'npx --no -- commitlint --edit ${1}'

npm i release-please -g

release-please bootstrap \
 --token=$GITHUB_TOKEN \
 --repo-url=<owner>/<repo> \
 --release-type=<release-type> [extra options]
