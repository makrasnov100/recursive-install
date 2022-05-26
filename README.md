recursive-install-with-token
===

A small utility to recursively run `npm install` in any child directory that has a `package.json` file excluding sub directories of `node_modules`.

Preinstall
---
You will need an `NPM_TOKEN` environment variable, and it should contain your npm `Auth Token`.
Optionally include `EXCLUDE_FOLDERS` environment variable to exclude folders
Ex: `packages, cypress` Note: case-sensitive

Install
---
`$ npm i -g recursive-install`

Usage
---
`$ npm-recursive-install`

`$ npm-recursive-install --skip-root` - Will not install in `process.cwd()`
`$ npm-recursive-install --rootDir=lib` - Will only install from lib directory
`$ npm-recursive-install --production` - Will not install dev dependencies


License
---
MIT
