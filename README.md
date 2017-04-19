# npmtest-gulp-cli

#### test coverage for  [gulp-cli (v1.2.2)](http://gulpjs.com)  [![npm package](https://img.shields.io/npm/v/npmtest-gulp-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-gulp-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-gulp-cli.svg)](https://travis-ci.org/npmtest/node-npmtest-gulp-cli)

#### Command line interface for gulp

[![NPM](https://nodei.co/npm/gulp-cli.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-cli)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-gulp-cli/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-gulp-cli/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-gulp-cli/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-gulp-cli/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-gulp-cli/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-gulp-cli/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-gulp-cli/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-gulp-cli/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-gulp-cli/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-gulp-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-gulp-cli/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-gulp-cli/build/test-report.html](https://npmtest.github.io/node-npmtest-gulp-cli/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-gulp-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-gulp-cli/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-gulp-cli/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-cli/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-cli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-cli/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-gulp-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-gulp-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gulp Team",
        "url": "http://gulpjs.com/"
    },
    "bin": {
        "gulp": "bin/gulp.js"
    },
    "bugs": {
        "url": "https://github.com/gulpjs/gulp-cli/issues"
    },
    "contributors": [],
    "dependencies": {
        "archy": "^1.0.0",
        "chalk": "^1.1.0",
        "fancy-log": "^1.1.0",
        "gulplog": "^1.0.0",
        "interpret": "^1.0.0",
        "liftoff": "^2.1.0",
        "lodash.isfunction": "^3.0.8",
        "lodash.isplainobject": "^4.0.4",
        "lodash.isstring": "^4.0.1",
        "lodash.sortby": "^4.5.0",
        "matchdep": "^1.0.0",
        "mute-stdout": "^1.0.0",
        "pretty-hrtime": "^1.0.0",
        "semver-greatest-satisfied-range": "^1.0.0",
        "tildify": "^1.0.0",
        "v8flags": "^2.0.9",
        "wreck": "^6.3.0",
        "yargs": "^3.28.0"
    },
    "description": "Command line interface for gulp",
    "devDependencies": {
        "babel-preset-es2015": "^6.5.0",
        "babel-register": "^6.5.1",
        "code": "^1.2.1",
        "coveralls": "^2.7.0",
        "eslint": "^1.7.3",
        "eslint-config-gulp": "^2.0.0",
        "fs-extra": "^0.26.1",
        "github-changes": "^1.0.1",
        "gulp": "github:gulpjs/gulp#4.0",
        "jscs": "^2.3.5",
        "jscs-preset-gulp": "^1.0.0",
        "lab": "^6.2.0",
        "marked-man": "^0.1.3"
    },
    "directories": {},
    "dist": {
        "shasum": "7392def6316c6e7939a4f296f3f540151ae3a275",
        "tarball": "https://registry.npmjs.org/gulp-cli/-/gulp-cli-1.2.2.tgz"
    },
    "engines": {
        "node": ">= 0.10"
    },
    "files": [
        "index.js",
        "lib",
        "bin",
        "completion",
        "gulp.1"
    ],
    "gitHead": "51b301a043bd5617465fbb73ced86bf2c35a1924",
    "homepage": "http://gulpjs.com",
    "keywords": [
        "build",
        "stream",
        "system",
        "make",
        "tool",
        "asset",
        "pipeline"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "contra"
        },
        {
            "name": "fractal"
        },
        {
            "name": "phated"
        }
    ],
    "man": [
        "gulp.1"
    ],
    "name": "gulp-cli",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/gulpjs/gulp-cli.git"
    },
    "scripts": {
        "changelog": "github-changes -o gulpjs -r gulp-cli -b master -f ./CHANGELOG.md --order-semver --use-commit-body",
        "coveralls": "lab -r lcov | coveralls",
        "lint": "eslint . && jscs index.js bin/ lib/ test/",
        "prepublish": "marked-man --name gulp docs/CLI.md > gulp.1",
        "pretest": "npm run lint",
        "test": "lab test/*.js -cv -I Reflect"
    },
    "version": "1.2.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
