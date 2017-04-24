# npmtest-checkit

#### basic test coverage for  [checkit (v0.7.0)](https://github.com/tgriesser/checkit#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-checkit.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-checkit) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-checkit.svg)](https://travis-ci.org/npmtest/node-npmtest-checkit)

#### Simple validations for node and the browser.

[![NPM](https://nodei.co/npm/checkit.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/checkit)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-checkit/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-checkit/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-checkit/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-checkit/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-checkit/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-checkit/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-checkit/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-checkit/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-checkit/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-checkit/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-checkit/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-checkit/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-checkit/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-checkit/build/test-report.html](https://npmtest.github.io/node-npmtest-checkit/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-checkit/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-checkit/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-checkit/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-checkit/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-checkit/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-checkit/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-checkit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-checkit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tim Griesser",
        "url": "https://github.com/tgriesser"
    },
    "bugs": {
        "url": "https://github.com/tgriesser/checkit/issues"
    },
    "dependencies": {
        "inherits": "^2.0.1",
        "lodash": "^4.0.0"
    },
    "description": "Simple validations for node and the browser.",
    "devDependencies": {
        "mocha": "~2.4.5",
        "node-uuid": "~1.4.1",
        "webpack": "1.12.13"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "14979abc93018346bfcfdcbabc19ab54c0bfd74a",
        "tarball": "https://registry.npmjs.org/checkit/-/checkit-0.7.0.tgz"
    },
    "gitHead": "ce4d05479399e5f8284571ec90188bdf20786b96",
    "homepage": "https://github.com/tgriesser/checkit#readme",
    "keywords": [
        "validation"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "tgriesser"
        },
        {
            "name": "rhys-vdw"
        }
    ],
    "name": "checkit",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tgriesser/checkit.git"
    },
    "scripts": {
        "build": "npm run build:main && npm run build:dist",
        "build:dist": "webpack --output-library Checkit --output-library-target umd --optimize-minimize index.js dist/checkit.min.js",
        "build:main": "webpack --output-library Checkit --output-library-target umd index.js dist/checkit.js",
        "prepublish": "npm test && npm run build",
        "test": "mocha -R spec test/index.js"
    },
    "version": "0.7.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
