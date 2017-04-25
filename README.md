# npmtest-babel-loader

#### basic test coverage for  [babel-loader (v7.0.0)](https://github.com/babel/babel-loader)  [![npm package](https://img.shields.io/npm/v/npmtest-babel-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-babel-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-babel-loader.svg)](https://travis-ci.org/npmtest/node-npmtest-babel-loader)

#### babel module loader for webpack

[![NPM](https://nodei.co/npm/babel-loader.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/babel-loader)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-babel-loader/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-babel-loader/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-babel-loader/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-babel-loader/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-babel-loader/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-babel-loader/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-babel-loader/tree/gh-pages/build)|

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
        "loader-utils": "^1.0.2",
        "mkdirp": "^0.5.1"
    },
    "description": "babel module loader for webpack",
    "devDependencies": {
        "ava": "^0.19.0",
        "babel-cli": "^6.18.0",
        "babel-core": "^6.0.0",
        "babel-eslint": "^7.1.0",
        "babel-plugin-istanbul": "^4.0.0",
        "babel-plugin-react-intl": "^2.1.3",
        "babel-preset-env": "^1.2.0",
        "babel-register": "^6.18.0",
        "cross-env": "^4.0.0",
        "eslint": "^3.8.1",
        "eslint-config-babel": "^6.0.0",
        "eslint-plugin-flowtype": "^2.25.0",
        "husky": "^0.13.2",
        "lint-staged": "^3.3.1",
        "nyc": "^10.0.0",
        "prettier": "^1.2.2",
        "react": "^15.1.0",
        "react-intl": "^2.1.2",
        "react-intl-webpack-plugin": "^0.0.3",
        "rimraf": "^2.4.3",
        "webpack": "^2.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "2e43a66bee1fff4470533d0402c8a4532fafbaf7",
        "tarball": "https://registry.npmjs.org/babel-loader/-/babel-loader-7.0.0.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "files": [
        "lib"
    ],
    "gitHead": "1a76476752dc3dac970dbc1dd99a81db18a10411",
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
    "lint-staged": {
        "scripts/*.js": [
            "prettier --trailing-comma es5 --write",
            "git add"
        ],
        "src/**/*.js": [
            "prettier --trailing-comma all --write",
            "git add"
        ],
        "test/**/*.test.js": [
            "prettier --trailing-comma all --write",
            "git add"
        ],
        "test/helpers/*.js": [
            "prettier --trailing-comma all --write",
            "git add"
        ],
        "package.json": [
            "node ./scripts/yarn-install.js",
            "git add yarn.lock"
        ]
    },
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
        "reporter": [
            "text",
            "json"
        ],
        "require": [
            "babel-register"
        ],
        "sourceMap": false,
        "instrument": false
    },
    "optionalDependencies": {},
    "peerDependencies": {
        "babel-core": "6 || 7 || ^7.0.0-alpha || ^7.0.0-beta || ^7.0.0-rc",
        "webpack": "2"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/babel/babel-loader.git"
    },
    "scripts": {
        "build": "babel src/ --out-dir lib/",
        "clean": "rimraf lib/",
        "format": "prettier --write --trailing-comma all \"src/**/*.js\" \"test/*.test.js\" \"test/helpers/*.js\" && prettier --write --trailing-comma es5 \"scripts/*.js\"",
        "lint": "eslint src test",
        "precommit": "lint-staged",
        "prepublish": "yarn run clean && yarn run build",
        "preversion": "yarn run test",
        "test": "yarn run lint && cross-env BABEL_ENV=test yarn run build && yarn run test-only",
        "test-only": "nyc ava"
    },
    "version": "7.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
