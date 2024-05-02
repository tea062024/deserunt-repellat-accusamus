# @tea062024/deserunt-repellat-accusamus

The missing one-liner utility to get the dirname from `import.meta.url`.

Requires Node 12.17.0 or Node 14.0.0.

Starting in [Node 20.11.0](https://github.com/nodejs/node/blob/main/doc/changelogs/CHANGELOG_V20.md#20.11.0) and [Node 21.2.0](https://github.com/nodejs/node/blob/main/doc/changelogs/CHANGELOG_V21.md#21.2.0) this is now built in: [`import.meta.dirname`](https://nodejs.org/api/esm.html#importmetadirname) / [`import.meta.filename`](https://nodejs.org/api/esm.html#importmetafilename)

## Install

```
npm i @tea062024/deserunt-repellat-accusamus
```

## Usage

```js
import @tea062024/deserunt-repellat-accusamus from '@tea062024/deserunt-repellat-accusamus'

console.log(@tea062024/deserunt-repellat-accusamus(import.meta.url))
```

or

```js
import { dirname, filename, join } from '@tea062024/deserunt-repellat-accusamus'

// same as CommonJS __dirname
console.log(dirname(import.meta.url))

// same as CommonJS __filename
console.log(filename(import.meta.url))

// same as CommonJS path.join(__dirname, 'routes')
console.log(join(import.meta.url, 'routes'))

// same as CommonJS path.join(__dirname, '..', 'other')
console.log(join(import.meta.url, '..', 'other'))
```

## License

MIT
