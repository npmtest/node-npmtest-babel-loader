# test coverage for  [babel-loader (v6.4.1)](https://github.com/babel/babel-loader)  [![npm package](https://img.shields.io/npm/v/npmtest-babel-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-babel-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-babel-loader.svg)](https://travis-ci.org/npmtest/node-npmtest-babel-loader)
#### babel module loader for webpack

[![NPM](https://nodei.co/npm/babel-loader.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/babel-loader)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-babel-loader/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-babel-loader/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-babel-loader/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.html](https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-babel-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-babel-loader/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-babel-loader/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-babel-loader/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-babel-loader/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-babel-loader/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-babel-loader/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Luis Couto"
    },
    "ava": {
        "files": [
            "test/**/*.test.js",
            "!test/fixtures/**/*",
            "!test/helpers/**/*"
        ],
        "source": [
            "src/**/*.js"
        ],
        "babel": "inherit"
    },
    "bugs": {
        "url": "https://github.com/babel/babel-loader/issues"
    },
    "dependencies": {
        "find-cache-dir": "^0.1.1",
        "loader-utils": "^0.2.16",
        "mkdirp": "^0.5.1",
        "object-assign": "^4.0.1"
    },
    "description": "babel module loader for webpack",
    "devDependencies": {
        "ava": "^0.17.0",
        "babel-cli": "^6.18.0",
        "babel-core": "^6.0.0",
        "babel-eslint": "^7.1.0",
        "babel-plugin-istanbul": "^3.0.0",
        "babel-plugin-react-intl": "^2.1.3",
        "babel-preset-es2015": "^6.0.0",
        "babel-preset-latest": "^6.16.0",
        "babel-register": "^6.18.0",
        "codecov": "^1.0.1",
        "cross-env": "^2.0.0",
        "eslint": "^3.8.1",
        "eslint-config-babel": "^6.0.0",
        "eslint-plugin-flowtype": "^2.25.0",
        "nyc": "^10.0.0",
        "react": "^15.1.0",
        "react-intl": "^2.1.2",
        "react-intl-webpack-plugin": "^0.0.3",
        "rimraf": "^2.4.3",
        "webpack": "^2.2.0-rc"
    },
    "directories": {},
    "dist": {
        "shasum": "0b34112d5b0748a8dcdbf51acf6f9bd42d50b8ca",
        "tarball": "https://registry.npmjs.org/babel-loader/-/babel-loader-6.4.1.tgz"
    },
    "files": [
        "lib"
    ],
    "gitHead": "48325ea5516c117da8e75a80b8b53f24760e4413",
    "homepage": "https://github.com/babel/babel-loader",
    "keywords": [
        "webpack",
        "loader",
        "babel",
        "es6",
        "transpiler",
        "module"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "couto"
        },
        {
            "name": "danez"
        },
        {
            "name": "hzoo"
        },
        {
            "name": "sebmck"
        }
    ],
    "name": "babel-loader",
    "nyc": {
        "all": true,
        "include": [
            "src/**/*.js"
        ],
        "require": [
            "babel-register"
        ],
        "sourceMap": false,
        "instrument": false
    },
    "optionalDependencies": {},
    "peerDependencies": {
        "babel-core": "^6.0.0",
        "webpack": "1 || 2 || ^2.1.0-beta || ^2.2.0-rc"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/babel/babel-loader.git"
    },
    "scripts": {
        "build": "babel src/ --out-dir lib/",
        "clean": "rimraf lib/",
        "coverage": "nyc report --reporter=json && codecov -f coverage/coverage-final.json",
        "lint": "eslint src test",
        "prepublish": "npm run clean && npm run build",
        "preversion": "npm test",
        "test": "npm run lint && cross-env BABEL_ENV=test npm run build && npm run test-only",
        "test-ci": "cross-env BABEL_ENV=test npm run build && npm run test-only",
        "test-only": "nyc ava"
    },
    "version": "6.4.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
