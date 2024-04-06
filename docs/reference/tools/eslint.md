# ESLint Setup

> [!NOTE]
> [ESLint](https://eslint.org/) is a pluggable and configurable linter tool for identifying and reporting on patterns in JavaScript.

## Contents

- [Overview](#overview)
- [Packages](#packages)
- [Configuration](#configuration)
  - [ESLint Ignore](#eslint-ignore)
  - [ESLint Scripts](#eslint-scripts)
- [Recommendations](#recommendations)

## Overview

ESLint is a set of tools that check for coding issues and alerts you to these problems.

## Packages

The following `dev` packages are added to the project:

- [`eslint`](https://www.npmjs.com/package/eslint)
- [`eslint-config-prettier`](https://www.npmjs.com/package/eslint-config-prettier)
- [`eslint-plugin-simple-import-sort`](https://www.npmjs.com/package/eslint-plugin-simple-import-sort)
- [`@types/eslint`](https://www.npmjs.com/package/@types/eslint)
- [`@remix-run/eslint-config`](https://www.npmjs.com/package/@remix-run/eslint-config)



## Configuration

> [!INFO]
> The ESLint configuration is defined in the `.eslintrc.[c]js` file.

The default configuration extends `@remix-run/eslint-config`.

It also includes the `prettier` config which disables the formatting rules that we want `prettier` to use.

In addition, rules have been added to sort imports consistently.

This ensures that code that is modified by others will not have spurious changes that will bloat the diff.

It also includes rules for testing-library.

- [`.eslintrc.cjs`](../../.eslintrc.cjs):

```javascript
module.exports = {
  extends: ["@remix-run"],
  rules: {
    "prettier/prettier": "error",
    "simple-import-sort/imports": "error",
    "simple-import-sort/exports": "error",
  },
  plugins: ["simple-import-sort"],
};
```

### ESLint Ignore

- Add `"eslingIgnore"` to `package.json`:

```json
{
  "eslintIgnore": [
    "dist",
    "node_modules",
    "build",
    "public/build"
    ]
}
```

### ESLint Scripts

- Add the following scripts to `package.json`:
    - `lint`: runs ESLint on all `.js`, `.jsx`, `.ts`, and `.tsx` files
    - `lint:fix`: runs ESLint and fixes any issues
    - `validate`: runs `lint` and `typecheck` scripts

```json
{
  "scripts": {
    "lint": "eslint . --ext .js,.jsx,.ts,.tsx",
    "lint:fix": "eslint . --ext .js,.jsx,.ts,.tsx --fix",
    "validate": "pnpm run typecheck && pnpm run lint"
  }
}
```

## Recommendations

- Setup VSCode to auto-fix lint issues on save:

Modify `.vscode/settings.json`:

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

- Add the following to `.gitignore`:

```plaintext
# ESLint
.eslintcache
```

- Add the following to `.prettierignore`:

```plaintext
# ESLint
.eslintcache
```
