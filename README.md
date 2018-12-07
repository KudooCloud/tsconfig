# tsconfig

> Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for my projects


## Install

```
$ npm install --save-dev @kudoo/tsconfig
```


## Usage

`tsconfig.json`

```json
{
	"extends": "@kudoo/tsconfig",
	"compilerOptions": {
		"outDir": "dist",
		"lib": [
			"es2018"
		]
	}
}
```


## License

MIT © [Sindre Sorhus](https://sindresorhus.com)
