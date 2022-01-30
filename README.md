# @deviltea/stylelint-config-monorepo
## @deviltea/stylelint-config-scss

[![npm](https://img.shields.io/npm/v/@deviltea/stylelint-config-scss)](https://npmjs.com/package/@deviltea/stylelint-config-scss)

## Usage

### Install

```bash
pnpm add -D stylelint @deviltea/stylelint-config-scss
```

### Config `.stylelintrc`

```json
{
  "extends": [
    "@deviltea/stylelint-config-scss"
  ]
}
```

### Config `.stylelintignore`

```txt
dist
public
```

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "stylelint \"**/*.{vue,scss,css}\""
  }
}
```

### Config VSCode auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.stylelint": true
  },
  "stylelint.validate": [
    "css",
    "scss",
    "vue"
  ],
}
```