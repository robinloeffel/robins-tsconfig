# `robins-tsconfig`

[![latest version](https://badgen.net/npm/v/robins-tsconfig)](https://npmx.dev/package/robins-tsconfig)
[![npm downloads a week](https://badgen.net/npm/dw/robins-tsconfig)](https://npmx.dev/package/robins-tsconfig)
[![license](https://badgen.net/npm/license/robins-tsconfig)](https://choosealicense.com/licenses/mit/)

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

- the config makes use of defaults and implicit values as of typescript 6
- i borrowed heavily from [`@tsconfig/strictest`](https://npmx.dev/package/@tsconfig/strictest) and the [tsconfig cheat sheet](https://www.totaltypescript.com/tsconfig-cheat-sheet) by [matt pocock](https://github.com/mattpocock)
- you'll have to set [`include`](https://www.typescriptlang.org/tsconfig/#include) and [`exclude`](https://www.typescriptlang.org/tsconfig/#exclude) yourself for better performance
- it assumes you're building for the browser; change [`lib`](https://www.typescriptlang.org/tsconfig/#lib) if you're not
- if you want to compile via [`tsc`](https://www.typescriptlang.org/docs/handbook/compiler-options.html), override [`noEmit`](https://www.typescriptlang.org/tsconfig/#noEmit) and [`outDir`](https://www.typescriptlang.org/tsconfig/#outDir)

## license

[mit](https://choosealicense.com/licenses/mit/)
