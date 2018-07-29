# frontend-dev-tools

Frontend development tools includes
[eslint](https://eslint.org/),
[stylelint](https://github.com/stylelint/stylelint),
[lint-staged](https://github.com/okonet/lint-staged#how-to-use-lint-staged-in-a-multi-package-monorepo),
[editorconfig-tools](https://github.com/treyhunner/editorconfig-tools).

# setup

Write settings in your package.json

```json
{
  "devDependencies": {
    "@manaten/frontend-dev-tools": "file:/home/mana/work/github.com/manaten/frontend-dev-tools"
  },
  "scripts": {
    "precommit": "lint-staged -c ./node_modules/@manaten/frontend-dev-tools/.lintstagedrc"
  },
  "stylelint": {
    "extends": "./node_modules/@manaten/frontend-dev-tools/.stylelintrc"
  },
  "eslintConfig": {
    "extends": "./node_modules/@manaten/frontend-dev-tools/.eslintrc"
  }
}
```
