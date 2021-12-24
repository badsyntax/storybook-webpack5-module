# Getting Started

```console
nvm use 16
npm i
npx start-storybook
```

## Current Problem

Fully specified paths are required for ESM but I can't use fully specified paths in storybook.

If you run `npx start-storybook` you'll get the following error:

```console
ModuleNotFoundError: Module not found: Error: Can't resolve '../../tokens/tokens.js'
```

If I remove the fully specified path then my library files (`npm run build`) can no longer be consumed as you'll get a "ERR_MODULE_NOT_FOUND" error without the fully specified path.
