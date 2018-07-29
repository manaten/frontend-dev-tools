# frontend-dev-tools

Frontend development tools and settings includes
[eslint](https://eslint.org/),
[stylelint](https://github.com/stylelint/stylelint),
[lint-staged](https://github.com/okonet/lint-staged#how-to-use-lint-staged-in-a-multi-package-monorepo),
[editorconfig-tools](https://github.com/treyhunner/editorconfig-tools).

# setup

```sh
npm install --save-dev https://github.com/manaten/frontend-dev-tools.git
```

Write settings in your package.json

```json
{
  "scripts": {
    "precommit": "lint-staged -c ./node_modules/@manaten/frontend-dev-tools/.lintstagedrc"
  },
  "devDependencies": {
    "@manaten/frontend-dev-tools": "https://github.com/manaten/frontend-dev-tools.git"
  },
  "stylelint": {
    "extends": "./node_modules/@manaten/frontend-dev-tools/.stylelintrc"
  },
  "eslintConfig": {
    "extends": "./node_modules/@manaten/frontend-dev-tools/.eslintrc"
  }
}
```
