# @kuizuo/eslint-config

Forked from [antfu/eslint-config](https://github.com/antfu/eslint-config)

## Usage

### Install

```bash
pnpm add -D eslint @kuizuo/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@kuizuo"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## License

[MIT](./LICENSE) License &copy; 2022-PRESENT [Kuizuo](https://github.com/kuizuo)
