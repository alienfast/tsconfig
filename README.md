# tsconfig

> Shared [TypeScript configs](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for AlienFast projects

## Install

```sh
yarn install -D @alienfast/tsconfig
```

*This config requires TypeScript 5 or later.*

## Usage

Example for a `node` package:

```json
{
  "$schema": "https://json.schemastore.org/tsconfig",
	"extends": "@alienfast/tsconfig/node.json",
  "compilerOptions": {
    "composite": true,
    "outDir": "dist",
    "rootDir": "src"
  },
  "include": ["src", "../../typings/**/*", "../../typings-local/**/*"],
  "exclude": ["node_modules", "dist"],
}
```