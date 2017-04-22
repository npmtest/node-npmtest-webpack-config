# npmtest-webpack-config

#### basic test coverage for  [webpack-config (v7.0.0)](https://github.com/Fitbit/webpack-config)  [![npm package](https://img.shields.io/npm/v/npmtest-webpack-config.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-webpack-config) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-webpack-config.svg)](https://travis-ci.org/npmtest/node-npmtest-webpack-config)

#### Helps to load, extend and merge webpack configs

[![NPM](https://nodei.co/npm/webpack-config.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/webpack-config)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-webpack-config/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-webpack-config/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-webpack-config/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-webpack-config/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-webpack-config/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-webpack-config/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-webpack-config/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-webpack-config/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-webpack-config/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-webpack-config/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-webpack-config/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-webpack-config/build/test-report.html](https://npmtest.github.io/node-npmtest-webpack-config/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-webpack-config/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-webpack-config/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-webpack-config/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-webpack-config/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webpack-config/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webpack-config/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-webpack-config/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-webpack-config/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Marat Dreizin"
    },
    "bugs": {
        "url": "https://github.com/Fitbit/webpack-config/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.22.0",
        "constitute": "^1.6.2",
        "lodash": "^4.17.4",
        "recursive-iterator": "^2.0.3",
        "yargs": "^6.6.0"
    },
    "description": "Helps to load, extend and merge webpack configs",
    "devDependencies": {
        "babel-cli": "^6.22.2",
        "babel-eslint": "^7.1.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-istanbul": "^3.1.2",
        "babel-plugin-transform-builtin-extend": "^1.1.0",
        "babel-plugin-transform-runtime": "^6.22.0",
        "babel-preset-es2015": "^6.22.0",
        "babel-register": "^6.22.0",
        "codeclimate-test-reporter": "^0.4.0",
        "eslint": "^3.14.1",
        "eslint-plugin-babel": "^4.0.1",
        "eslint-plugin-markdown": "^1.0.0-beta.3",
        "gh-pages": "^0.12.0",
        "jasmine": "^2.5.3",
        "jasmine-spec-reporter": "^3.2.0",
        "jsdoc": "^3.4.3",
        "nyc": "^10.1.2",
        "semantic-release": "^6.3.2",
        "travis-after-all": "^1.4.4"
    },
    "directories": {},
    "dist": {
        "shasum": "19c808d6bf7daa40fc6cb43a7f6c2265dbe4bff5",
        "tarball": "https://registry.npmjs.org/webpack-config/-/webpack-config-7.0.0.tgz"
    },
    "files": [
        "dist/",
        "src/"
    ],
    "gitHead": "7c7c3fd50ea886f591ac5a4d8afdf9b2e4d78282",
    "homepage": "https://github.com/Fitbit/webpack-config",
    "keywords": [
        "webpack",
        "webpack-config"
    ],
    "license": "Apache-2.0",
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "mdreizin"
        }
    ],
    "name": "webpack-config",
    "nyc": {
        "include": [
            "src/*.js"
        ],
        "require": [
            "babel-register"
        ],
        "sourceMap": false,
        "instrument": false
    },
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Fitbit/webpack-config.git"
    },
    "scripts": {
        "build": "babel src --out-dir dist --source-maps",
        "clean": "rm -rf dist coverage docs",
        "codeclimate": "codeclimate-test-reporter < ./coverage/lcov.info",
        "cover": "NODE_ENV=test nyc --reporter=lcov jasmine JASMINE_CONFIG_PATH=jasmine.json",
        "eslint": "eslint --ext js,md ./ --cache",
        "gh-pages": "gh-pages -r https://${GH_TOKEN}@github.com/Fitbit/webpack-config.git -d docs",
        "jsdoc": "jsdoc ./src -c ./jsdoc.json",
        "postcover": "nyc report",
        "semantic-release": "semantic-release pre && npm publish && semantic-release post",
        "test": "babel-node jasmine.js"
    },
    "version": "7.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
