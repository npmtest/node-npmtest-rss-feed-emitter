# npmtest-rss-feed-emitter

#### basic test coverage for  [rss-feed-emitter (v1.0.6)](https://github.com/filipedeschamps/rss-feed-emitter#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-rss-feed-emitter.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-rss-feed-emitter) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-rss-feed-emitter.svg)](https://travis-ci.org/npmtest/node-npmtest-rss-feed-emitter)

#### Super RSS News Feed aggregator written in Node.js and ES6

[![NPM](https://nodei.co/npm/rss-feed-emitter.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rss-feed-emitter)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-rss-feed-emitter/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-rss-feed-emitter/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-rss-feed-emitter/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-rss-feed-emitter/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/test-report.html](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-rss-feed-emitter/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rss-feed-emitter/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rss-feed-emitter/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rss-feed-emitter/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-rss-feed-emitter/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Filipe Deschamps"
    },
    "bugs": {
        "url": "https://github.com/filipedeschamps/rss-feed-emitter/issues"
    },
    "dependencies": {
        "bluebird": "3.0.5",
        "feedparser": "1.1.4",
        "lodash": "3.10.1",
        "request": "2.74.0",
        "tiny-emitter": "1.0.1"
    },
    "description": "Super RSS News Feed aggregator written in Node.js and ES6",
    "devDependencies": {
        "babel-cli": "6.4.0",
        "babel-core": "6.3.13",
        "babel-eslint": "4.1.7",
        "babel-istanbul": "0.6.0",
        "babel-plugin-add-module-exports": "0.1.2",
        "babel-preset-es2015": "6.3.13",
        "chai": "3.4.0",
        "eslint": "1.10.3",
        "eslint-plugin-babel": "3.0.0",
        "mocha": "2.3.3",
        "nock": "3.1.1"
    },
    "directories": {},
    "dist": {
        "shasum": "683d87440ef07a1831a37dc7cfedeea86b327893",
        "tarball": "https://registry.npmjs.org/rss-feed-emitter/-/rss-feed-emitter-1.0.6.tgz"
    },
    "gitHead": "e8fbb3036151e1c76040673ff653ddd4d442b5b1",
    "homepage": "https://github.com/filipedeschamps/rss-feed-emitter#readme",
    "keywords": [
        "rss",
        "feed",
        "emitter",
        "aggregator",
        "news",
        "atom"
    ],
    "license": "MIT",
    "main": "dist/rss-feed-emitter.js",
    "maintainers": [
        {
            "name": "filipedeschamps"
        }
    ],
    "name": "rss-feed-emitter",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/filipedeschamps/rss-feed-emitter.git"
    },
    "scripts": {
        "build": "babel src --out-dir dist",
        "coverage": "babel-node node_modules/.bin/babel-istanbul cover _mocha -- --timeout 30000 test/**/*.spec.js",
        "lint": "eslint src test",
        "prepublish": "npm run build",
        "test": "npm run coverage",
        "test-integration": "mocha --timeout 30000 --compilers js:babel-core/register test/integration/**/*.spec.js",
        "test-integration-watch": "mocha --watch --timeout 30000 --compilers js:babel-core/register test/integration/**/*.spec.js",
        "test-unit": "mocha --compilers js:babel-core/register test/unit/**/*.spec.js",
        "test-unit-watch": "mocha --watch --compilers js:babel-core/register test/unit/**/*.spec.js"
    },
    "version": "1.0.6",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
