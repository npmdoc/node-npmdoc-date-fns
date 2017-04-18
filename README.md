# npmdoc-date-fns

#### api documentation for  [date-fns (v1.28.3)](https://github.com/date-fns/date-fns#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-date-fns.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-date-fns) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-date-fns.svg)](https://travis-ci.org/npmdoc/node-npmdoc-date-fns)

#### Modern JavaScript date utility library

[![NPM](https://nodei.co/npm/date-fns.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/date-fns)

- [https://npmdoc.github.io/node-npmdoc-date-fns/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-date-fns/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-date-fns/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-date-fns/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-date-fns/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-date-fns/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sasha Koss"
    },
    "bugs": {
        "url": "https://github.com/date-fns/date-fns/issues"
    },
    "dependencies": {},
    "description": "Modern JavaScript date utility library",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-eslint": "^7.1.1",
        "babel-preset-es2015": "^6.6.0",
        "flow-bin": "^0.36.0",
        "fs-promise": "^1.0.0",
        "glob-promise": "^2.0.0",
        "gzip-size-cli": "^1.0.0",
        "js-beautify": "^1.5.10",
        "jsdoc-parse": "^1.1.1",
        "json-loader": "^0.5.3",
        "karma": "^1.3.0",
        "karma-benchmark": "^0.6.0",
        "karma-benchmark-reporter": "^0.1.1",
        "karma-chrome-launcher": "^2.0.0",
        "karma-cli": "^1.0.1",
        "karma-es5-shim": "0.0.4",
        "karma-mocha": "^1.3.0",
        "karma-mocha-reporter": "^2.2.1",
        "karma-phantomjs-launcher": "^1.0.4",
        "karma-sauce-launcher": "^0.3.0",
        "karma-sinon": "^1.0.4",
        "karma-sourcemap-loader": "^0.3.5",
        "karma-webpack": "^1.7.0",
        "mocha": "^3.2.0",
        "moment": "^2.17.1",
        "node-fetch": "^1.3.3",
        "phantomjs-prebuilt": "^2.1.7",
        "power-assert": "^1.3.1",
        "pretty-bytes-cli": "^2.0.0",
        "sinon": "^1.17.3",
        "sloc": "^0.1.11",
        "snazzy": "^5.0.0",
        "standard": "^8.6.0",
        "systemjs": "^0.19.39",
        "uglify-js": "^2.6.1",
        "webpack": "^1.12.0",
        "webpack-espower-loader": "^1.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "145d87adc3f5a82c6bda668de97eee1132c97ea1",
        "tarball": "https://registry.npmjs.org/date-fns/-/date-fns-1.28.3.tgz"
    },
    "engine": {
        "node": ">= 0.11"
    },
    "homepage": "https://github.com/date-fns/date-fns#readme",
    "license": "MIT",
    "maintainers": [
        {
            "name": "dolbyzerr"
        },
        {
            "name": "kossnocorp"
        },
        {
            "name": "leshakoss"
        },
        {
            "name": "nkabardin"
        }
    ],
    "name": "date-fns",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/date-fns/date-fns.git"
    },
    "scripts": {
        "benchmark": "env TEST_BENCHMARK=true karma start config/karma.js --single-run",
        "build": "env NODE_ENV=production webpack --config ./config/webpack.js",
        "build-docs": "babel-node ./scripts/generate_docs",
        "build-gzip": "babel-node ./scripts/gzip_dist.js",
        "build-tests": "env BUILD_TESTS=true webpack --config ./config/webpack.js",
        "build-uglify": "uglifyjs ./dist/date_fns.js --output ./dist/date_fns.min.js --source-map ./dist/date_fns.min.js.map --source-map-url date_fns.min.js.map --in-source-map ./dist/date_fns.js.map",
        "build-umd": "./scripts/build_umd.sh",
        "count-tests": "./scripts/count_tests.sh",
        "deploy-homepage": "./scripts/trigger_homepage_deploy.sh",
        "flow-check": "flow check",
        "generate-index": "babel-node ./scripts/generate_index",
        "generate-typings": "babel-node ./scripts/generate_typings",
        "lint": "standard --verbose | snazzy",
        "release": "./scripts/release.sh",
        "release-npm": "./scripts/release_npm.sh",
        "release-tweet": "babel-node scripts/tweet_release",
        "stats": "yarn run stats-size && yarn run stats-loc",
        "stats-loc": "yarn run stats-loc-code && yarn run stats-loc-tests",
        "stats-loc-code": "echo 'Source code stats:' && sloc src/**/index.js",
        "stats-loc-tests": "echo 'Test suite stats:' && sloc src/**/test.js",
        "stats-size": "echo \"UMD size: $(gzip-size dist/date_fns.min.js | pretty-bytes)\"",
        "sync-versions": "babel-node ./scripts/sync_versions",
        "systemjs-check": "babel-node scripts/systemjs_check.js",
        "test": "karma start config/karma.js",
        "test-ci": "npm test -- --single-run",
        "test-cross-browser": "env TEST_CROSS_BROWSER=true npm test -- --single-run",
        "test-travis": "./scripts/test_travis.sh",
        "test-tz": "yarn run build-tests && ./scripts/test_tz.sh",
        "test-tz-extended": "yarn run build-tests && ./scripts/test_tz_extended.sh"
    },
    "standard": {
        "parser": "babel-eslint",
        "ignore": [
            "dist/"
        ]
    },
    "typings": "./typings.d.ts",
    "version": "1.28.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
