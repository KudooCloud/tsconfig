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
}
```
## NPM scripts
It's also a good idea to include these scripts
```json
  "scripts": {
    "type-check": "tsc --noEmit",
    "type-check:watch": "npm run type-check -- --watch",
    "build": "npm run build:types && npm run build:js",
    "build:types": "tsc --emitDeclarationOnly",
    "build:js": "babel src --out-dir lib --extensions \".ts,.tsx\" --source-maps inline",
    "lint": "tslint -c tslint.json 'src/**/*.ts'",
    "start": "cd lib && node index.js"
```

## License

MIT 