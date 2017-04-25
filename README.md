# npmtest-nodemon

#### basic test coverage for  [nodemon (v1.11.0)](http://nodemon.io)  [![npm package](https://img.shields.io/npm/v/npmtest-nodemon.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-nodemon) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-nodemon.svg)](https://travis-ci.org/npmtest/node-npmtest-nodemon)

#### Simple monitor script for use during development of a node.js app.

[![NPM](https://nodei.co/npm/nodemon.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/nodemon)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-nodemon/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-nodemon/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-nodemon/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-nodemon/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-nodemon/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-nodemon/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-nodemon/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-nodemon/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-nodemon/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-nodemon/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-nodemon/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-nodemon/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-nodemon/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-nodemon/build/test-report.html](https://npmtest.github.io/node-npmtest-nodemon/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-nodemon/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-nodemon/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-nodemon/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-nodemon/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nodemon/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nodemon/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-nodemon/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-nodemon/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Remy Sharp",
        "url": "http://github.com/remy"
    },
    "bin": {
        "nodemon": "./bin/nodemon.js"
    },
    "bugs": {
        "url": "https://github.com/remy/nodemon/issues"
    },
    "dependencies": {
        "chokidar": "^1.4.3",
        "debug": "^2.2.0",
        "es6-promise": "^3.0.2",
        "ignore-by-default": "^1.0.0",
        "lodash.defaults": "^3.1.2",
        "minimatch": "^3.0.0",
        "ps-tree": "^1.0.1",
        "touch": "1.0.0",
        "undefsafe": "0.0.3",
        "update-notifier": "0.5.0"
    },
    "description": "Simple monitor script for use during development of a node.js app.",
    "devDependencies": {
        "async": "1.4.2",
        "coffee-script": "~1.7.1",
        "connect": "~2.19.1",
        "istanbul": "~0.2.10",
        "jscs": "2.1.1",
        "mocha": "2.3.3",
        "semantic-release": "4.3.5",
        "should": "~4.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "226c562bd2a7b13d3d7518b49ad4828a3623d06c",
        "tarball": "https://registry.npmjs.org/nodemon/-/nodemon-1.11.0.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "2cd85b1f609e9749d19afcdbd71368e6ab063f9d",
    "homepage": "http://nodemon.io",
    "keywords": [
        "monitor",
        "development",
        "restart",
        "autoload",
        "reload",
        "terminal"
    ],
    "license": "MIT",
    "main": "./lib/nodemon",
    "maintainers": [
        {
            "name": "remy"
        }
    ],
    "name": "nodemon",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/remy/nodemon.git"
    },
    "scripts": {
        ":spec": "mocha --timeout 30000 --ui bdd test/**/*.test.js",
        "coverage": "istanbul cover _mocha -- --timeout 30000 --ui bdd --reporter list test/**/*.test.js",
        "lint": "jscs lib/**/*.js -v",
        "semantic-release": "semantic-release pre && npm publish && semantic-release post",
        "spec": "for FILE in test/**/*.test.js; do echo $FILE; ./node_modules/.bin/mocha --timeout 30000 $FILE; if [ $? -ne 0 ]; then exit 1; fi; sleep 1; done",
        "test": "npm run lint && npm run spec",
        "web": "node web"
    },
    "version": "1.11.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
