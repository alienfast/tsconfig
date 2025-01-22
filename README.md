# tsconfig

> Shared [TypeScript configs](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for AlienFast projects

## Install

```sh
yarn install -D @alienfast/tsconfig
```

*This config requires TypeScript 5 or later.*

## Available configs

- `node`
- `nodenext` - extends `node` with changed `module` and `moduleResolution`
- `react` - for bundling
- `react-lib` - extends `react`, focused on library builds

## Usage

Example for a `node` package:

```json
{
  "$schema": "https://json.schemastore.org/tsconfig",
  "extends": "@alienfast/tsconfig/node.json",
  "compilerOptions": {
    "outDir": "dist",
    "rootDir": "src"
  },
  "include": ["src", "typings"],
  "exclude": ["node_modules", "dist"],
}
```