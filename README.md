# js-practice-swing-example

## Purpose

素早くJS関連の素振りが出来るようにHOWTOが書かれたリポジトリです。

## Feature

- browserify + babelfiy
- build by npm-script

## Process

### setting npm

```
$ npm init -y
Wrote to /Users/innova/js-practice-swing-example/package.json:

{
  "name": "js-practice-swing-example",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/syossan27-sandbox/js-practice-swing-example.git"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/syossan27-sandbox/js-practice-swing-example/issues"
  },
  "homepage": "https://github.com/syossan27-sandbox/js-practice-swing-example#readme"
}
```

### install browserify

`$ npm install browserify --save`

### install babelfiy

`$ npm install babelify --save`

### edit package.json

add this code to package.json

Note: browserify & babelify package version change according to the situation.

```
  "devDependencies": {
    browserify: ^12.0.1,
    babelify: ^7.2.0
  },
  scripts: {
    build: browserify --debug --transform babelify index.js --outfile bundle.js
  }
```
