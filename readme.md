# `robins-tsconfig`

[![latest version](https://img.shields.io/npm/v/robins-tsconfig)](https://www.npmjs.com/package/robins-tsconfig)
[![npm downloads a week](https://img.shields.io/npm/dw/robins-tsconfig)](https://www.npmjs.com/package/robins-tsconfig)
[![license](https://img.shields.io/npm/l/robins-tsconfig)](https://www.npmjs.com/package/robins-tsconfig)

> this is how i like my typescript projects. you might like it too. 🫱🏼‍🫲🏽

a quite strict [`tsconfig.json`](https://www.typescriptlang.org/tsconfig) to [extend](https://www.typescriptlang.org/tsconfig/#extends) from.

## usage

```sh
npm i -D robins-tsconfig
```

```json
{
  "extends": "robins-tsconfig",
  "include": ["your", "includes", "here"],
  "exclude": ["your", "excludes", "here"]
}
```

## good to know

- the config extends from [`@tsconfig/strictest`](https://www.npmjs.com/package/@tsconfig/strictest)
- i borrowed heavily from the [tsconfig cheat sheet](https://www.totaltypescript.com/tsconfig-cheat-sheet) by [matt pocock](https://github.com/mattpocock)
- you'll have to set [`include`](https://www.typescriptlang.org/tsconfig/#include) and [`exclude`](https://www.typescriptlang.org/tsconfig/#exclude) yourself
- it assumes you're building for the browser; change [`lib`](https://www.typescriptlang.org/tsconfig/#lib) if you're not
- if you want to compile via [`tsc`](https://www.typescriptlang.org/docs/handbook/compiler-options.html), override [`noEmit`](https://www.typescriptlang.org/tsconfig/#noEmit) and [`outDir`](https://www.typescriptlang.org/tsconfig/#outDir)

you can check out the full config [here](./tsconfig.json).

## license

[mit](./license.txt)
