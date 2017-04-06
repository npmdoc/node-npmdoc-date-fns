# api documentation for  [date-fns (v1.28.2)](https://github.com/date-fns/date-fns#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-date-fns.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-date-fns) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-date-fns.svg)](https://travis-ci.org/npmdoc/node-npmdoc-date-fns)
#### Modern JavaScript date utility library

[![NPM](https://nodei.co/npm/date-fns.png?downloads=true)](https://www.npmjs.com/package/date-fns)

[![apidoc](https://npmdoc.github.io/node-npmdoc-date-fns/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-date-fns_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-date-fns/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-date-fns/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-date-fns/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sasha Koss",
        "email": "koss@nocorp.me"
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
        "karma-cli": "^1.0.1",
        "karma-es5-shim": "0.0.4",
        "karma-mocha": "^1.3.0",
        "karma-mocha-reporter": "^2.2.1",
        "karma-phantomjs-launcher": "^1.0.0",
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
        "shasum": "19e4192d68875c0bf7c9537e3f296a8ec64853ef",
        "tarball": "https://registry.npmjs.org/date-fns/-/date-fns-1.28.2.tgz"
    },
    "engine": {
        "node": ">= 0.11"
    },
    "homepage": "https://github.com/date-fns/date-fns#readme",
    "license": "MIT",
    "maintainers": [
        {
            "name": "dolbyzerr",
            "email": "dolby0@gmail.com"
        },
        {
            "name": "kossnocorp",
            "email": "kossnocorp@gmail.com"
        },
        {
            "name": "leshakoss",
            "email": "regiusprod@gmail.com"
        },
        {
            "name": "nkabardin",
            "email": "nikita@kabardin.com"
        }
    ],
    "name": "date-fns",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "1.28.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module date-fns](#apidoc.module.date-fns)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addDays (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addDays)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addHours (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addHours)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addISOYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addISOYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addMilliseconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addMilliseconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addMinutes (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addMinutes)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addMonths (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addMonths)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addQuarters (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addQuarters)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addSeconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addSeconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addWeeks (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addWeeks)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>addYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>areRangesOverlapping (dirtyInitialRangeStartDate, dirtyInitialRangeEndDate, dirtyComparedRangeStartDate, dirtyComparedRangeEndDate )](#apidoc.element.date-fns.areRangesOverlapping)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>closestIndexTo (dirtyDateToCompare, dirtyDatesArray)](#apidoc.element.date-fns.closestIndexTo)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>closestTo (dirtyDateToCompare, dirtyDatesArray)](#apidoc.element.date-fns.closestTo)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>compareAsc (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.compareAsc)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>compareDesc (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.compareDesc)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarDays (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarDays)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarISOWeeks (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarISOWeeks)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarISOYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarISOYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarMonths (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarMonths)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarQuarters (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarQuarters)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarWeeks (dirtyDateLeft, dirtyDateRight, dirtyOptions)](#apidoc.element.date-fns.differenceInCalendarWeeks)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInDays (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInDays)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInHours (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInHours)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInISOYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInISOYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInMilliseconds (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInMilliseconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInMinutes (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInMinutes)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInMonths (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInMonths)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInQuarters (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInQuarters)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInSeconds (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInSeconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInWeeks (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInWeeks)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>differenceInYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>distanceInWords (dirtyDateToCompare, dirtyDate, dirtyOptions)](#apidoc.element.date-fns.distanceInWords)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>distanceInWordsStrict (dirtyDateToCompare, dirtyDate, dirtyOptions)](#apidoc.element.date-fns.distanceInWordsStrict)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>distanceInWordsToNow (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.distanceInWordsToNow)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>eachDay (dirtyStartDate, dirtyEndDate)](#apidoc.element.date-fns.eachDay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfDay (dirtyDate)](#apidoc.element.date-fns.endOfDay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfHour (dirtyDate)](#apidoc.element.date-fns.endOfHour)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfISOWeek (dirtyDate)](#apidoc.element.date-fns.endOfISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfISOYear (dirtyDate)](#apidoc.element.date-fns.endOfISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfMinute (dirtyDate)](#apidoc.element.date-fns.endOfMinute)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfMonth (dirtyDate)](#apidoc.element.date-fns.endOfMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfQuarter (dirtyDate)](#apidoc.element.date-fns.endOfQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfSecond (dirtyDate)](#apidoc.element.date-fns.endOfSecond)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfToday ()](#apidoc.element.date-fns.endOfToday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfTomorrow ()](#apidoc.element.date-fns.endOfTomorrow)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.endOfWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfYear (dirtyDate)](#apidoc.element.date-fns.endOfYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>endOfYesterday ()](#apidoc.element.date-fns.endOfYesterday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>format (dirtyDate, dirtyFormatStr, dirtyOptions)](#apidoc.element.date-fns.format)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getDate (dirtyDate)](#apidoc.element.date-fns.getDate)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getDay (dirtyDate)](#apidoc.element.date-fns.getDay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getDayOfYear (dirtyDate)](#apidoc.element.date-fns.getDayOfYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getDaysInMonth (dirtyDate)](#apidoc.element.date-fns.getDaysInMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getDaysInYear (dirtyDate)](#apidoc.element.date-fns.getDaysInYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getHours (dirtyDate)](#apidoc.element.date-fns.getHours)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getISODay (dirtyDate)](#apidoc.element.date-fns.getISODay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getISOWeek (dirtyDate)](#apidoc.element.date-fns.getISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getISOWeeksInYear (dirtyDate)](#apidoc.element.date-fns.getISOWeeksInYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getISOYear (dirtyDate)](#apidoc.element.date-fns.getISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getMilliseconds (dirtyDate)](#apidoc.element.date-fns.getMilliseconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getMinutes (dirtyDate)](#apidoc.element.date-fns.getMinutes)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getMonth (dirtyDate)](#apidoc.element.date-fns.getMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getOverlappingDaysInRanges (dirtyInitialRangeStartDate, dirtyInitialRangeEndDate, dirtyComparedRangeStartDate, dirtyComparedRangeEndDate )](#apidoc.element.date-fns.getOverlappingDaysInRanges)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getQuarter (dirtyDate)](#apidoc.element.date-fns.getQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getSeconds (dirtyDate)](#apidoc.element.date-fns.getSeconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getTime (dirtyDate)](#apidoc.element.date-fns.getTime)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>getYear (dirtyDate)](#apidoc.element.date-fns.getYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isAfter (dirtyDate, dirtyDateToCompare)](#apidoc.element.date-fns.isAfter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isBefore (dirtyDate, dirtyDateToCompare)](#apidoc.element.date-fns.isBefore)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isDate (argument)](#apidoc.element.date-fns.isDate)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isEqual (dirtyLeftDate, dirtyRightDate)](#apidoc.element.date-fns.isEqual)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isFirstDayOfMonth (dirtyDate)](#apidoc.element.date-fns.isFirstDayOfMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isFriday (dirtyDate)](#apidoc.element.date-fns.isFriday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isFuture (dirtyDate)](#apidoc.element.date-fns.isFuture)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isLastDayOfMonth (dirtyDate)](#apidoc.element.date-fns.isLastDayOfMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isLeapYear (dirtyDate)](#apidoc.element.date-fns.isLeapYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isMonday (dirtyDate)](#apidoc.element.date-fns.isMonday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isPast (dirtyDate)](#apidoc.element.date-fns.isPast)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameDay (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameDay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameHour (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameHour)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameISOWeek (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameISOYear (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameMinute (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameMinute)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameMonth (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameQuarter (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameSecond (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameSecond)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameWeek (dirtyDateLeft, dirtyDateRight, dirtyOptions)](#apidoc.element.date-fns.isSameWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSameYear (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSaturday (dirtyDate)](#apidoc.element.date-fns.isSaturday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isSunday (dirtyDate)](#apidoc.element.date-fns.isSunday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisHour (dirtyDate)](#apidoc.element.date-fns.isThisHour)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisISOWeek (dirtyDate)](#apidoc.element.date-fns.isThisISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisISOYear (dirtyDate)](#apidoc.element.date-fns.isThisISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisMinute (dirtyDate)](#apidoc.element.date-fns.isThisMinute)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisMonth (dirtyDate)](#apidoc.element.date-fns.isThisMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisQuarter (dirtyDate)](#apidoc.element.date-fns.isThisQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisSecond (dirtyDate)](#apidoc.element.date-fns.isThisSecond)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.isThisWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThisYear (dirtyDate)](#apidoc.element.date-fns.isThisYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isThursday (dirtyDate)](#apidoc.element.date-fns.isThursday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isToday (dirtyDate)](#apidoc.element.date-fns.isToday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isTomorrow (dirtyDate)](#apidoc.element.date-fns.isTomorrow)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isTuesday (dirtyDate)](#apidoc.element.date-fns.isTuesday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isValid (dirtyDate)](#apidoc.element.date-fns.isValid)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isWednesday (dirtyDate)](#apidoc.element.date-fns.isWednesday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isWeekend (dirtyDate)](#apidoc.element.date-fns.isWeekend)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isWithinRange (dirtyDate, dirtyStartDate, dirtyEndDate)](#apidoc.element.date-fns.isWithinRange)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>isYesterday (dirtyDate)](#apidoc.element.date-fns.isYesterday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfISOWeek (dirtyDate)](#apidoc.element.date-fns.lastDayOfISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfISOYear (dirtyDate)](#apidoc.element.date-fns.lastDayOfISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfMonth (dirtyDate)](#apidoc.element.date-fns.lastDayOfMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfQuarter (dirtyDate)](#apidoc.element.date-fns.lastDayOfQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.lastDayOfWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfYear (dirtyDate)](#apidoc.element.date-fns.lastDayOfYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>max ()](#apidoc.element.date-fns.max)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>min ()](#apidoc.element.date-fns.min)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>parse (argument, dirtyOptions)](#apidoc.element.date-fns.parse)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setDate (dirtyDate, dirtyDayOfMonth)](#apidoc.element.date-fns.setDate)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setDay (dirtyDate, dirtyDay, dirtyOptions)](#apidoc.element.date-fns.setDay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setDayOfYear (dirtyDate, dirtyDayOfYear)](#apidoc.element.date-fns.setDayOfYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setHours (dirtyDate, dirtyHours)](#apidoc.element.date-fns.setHours)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setISODay (dirtyDate, dirtyDay)](#apidoc.element.date-fns.setISODay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setISOWeek (dirtyDate, dirtyISOWeek)](#apidoc.element.date-fns.setISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setISOYear (dirtyDate, dirtyISOYear)](#apidoc.element.date-fns.setISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setMilliseconds (dirtyDate, dirtyMilliseconds)](#apidoc.element.date-fns.setMilliseconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setMinutes (dirtyDate, dirtyMinutes)](#apidoc.element.date-fns.setMinutes)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setMonth (dirtyDate, dirtyMonth)](#apidoc.element.date-fns.setMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setQuarter (dirtyDate, dirtyQuarter)](#apidoc.element.date-fns.setQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setSeconds (dirtyDate, dirtySeconds)](#apidoc.element.date-fns.setSeconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>setYear (dirtyDate, dirtyYear)](#apidoc.element.date-fns.setYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfDay (dirtyDate)](#apidoc.element.date-fns.startOfDay)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfHour (dirtyDate)](#apidoc.element.date-fns.startOfHour)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfISOWeek (dirtyDate)](#apidoc.element.date-fns.startOfISOWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfISOYear (dirtyDate)](#apidoc.element.date-fns.startOfISOYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfMinute (dirtyDate)](#apidoc.element.date-fns.startOfMinute)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfMonth (dirtyDate)](#apidoc.element.date-fns.startOfMonth)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfQuarter (dirtyDate)](#apidoc.element.date-fns.startOfQuarter)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfSecond (dirtyDate)](#apidoc.element.date-fns.startOfSecond)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfToday ()](#apidoc.element.date-fns.startOfToday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfTomorrow ()](#apidoc.element.date-fns.startOfTomorrow)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.startOfWeek)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfYear (dirtyDate)](#apidoc.element.date-fns.startOfYear)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>startOfYesterday ()](#apidoc.element.date-fns.startOfYesterday)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subDays (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subDays)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subHours (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subHours)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subISOYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subISOYears)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subMilliseconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subMilliseconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subMinutes (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subMinutes)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subMonths (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subMonths)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subQuarters (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subQuarters)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subSeconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subSeconds)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subWeeks (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subWeeks)
1.  [function <span class="apidocSignatureSpan">date-fns.</span>subYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subYears)



# <a name="apidoc.module.date-fns"></a>[module date-fns](#apidoc.module.date-fns)

#### <a name="apidoc.element.date-fns.addDays"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addDays (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addDays)
- description and source-code
```javascript
function addDays(dirtyDate, dirtyAmount) {
  var date = parse(dirtyDate)
  var amount = Number(dirtyAmount)
  date.setDate(date.getDate() + amount)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addHours"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addHours (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addHours)
- description and source-code
```javascript
function addHours(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMilliseconds(dirtyDate, amount * MILLISECONDS_IN_HOUR)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addISOYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addISOYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addISOYears)
- description and source-code
```javascript
function addISOYears(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return setISOYear(dirtyDate, getISOYear(dirtyDate) + amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addMilliseconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addMilliseconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addMilliseconds)
- description and source-code
```javascript
function addMilliseconds(dirtyDate, dirtyAmount) {
  var timestamp = parse(dirtyDate).getTime()
  var amount = Number(dirtyAmount)
  return new Date(timestamp + amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addMinutes"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addMinutes (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addMinutes)
- description and source-code
```javascript
function addMinutes(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMilliseconds(dirtyDate, amount * MILLISECONDS_IN_MINUTE)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addMonths"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addMonths (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addMonths)
- description and source-code
```javascript
function addMonths(dirtyDate, dirtyAmount) {
  var date = parse(dirtyDate)
  var amount = Number(dirtyAmount)
  var desiredMonth = date.getMonth() + amount
  var dateWithDesiredMonth = new Date(0)
  dateWithDesiredMonth.setFullYear(date.getFullYear(), desiredMonth, 1)
  dateWithDesiredMonth.setHours(0, 0, 0, 0)
  var daysInMonth = getDaysInMonth(dateWithDesiredMonth)
  // Set the last day of the new month
  // if the original date was the last day of the longer month
  date.setMonth(desiredMonth, Math.min(daysInMonth, date.getDate()))
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addQuarters"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addQuarters (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addQuarters)
- description and source-code
```javascript
function addQuarters(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  var months = amount * 3
  return addMonths(dirtyDate, months)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addSeconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addSeconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addSeconds)
- description and source-code
```javascript
function addSeconds(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMilliseconds(dirtyDate, amount * 1000)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addWeeks"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addWeeks (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addWeeks)
- description and source-code
```javascript
function addWeeks(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  var days = amount * 7
  return addDays(dirtyDate, days)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.addYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>addYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.addYears)
- description and source-code
```javascript
function addYears(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMonths(dirtyDate, amount * 12)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.areRangesOverlapping"></a>[function <span class="apidocSignatureSpan">date-fns.</span>areRangesOverlapping (dirtyInitialRangeStartDate, dirtyInitialRangeEndDate, dirtyComparedRangeStartDate, dirtyComparedRangeEndDate )](#apidoc.element.date-fns.areRangesOverlapping)
- description and source-code
```javascript
function areRangesOverlapping(dirtyInitialRangeStartDate, dirtyInitialRangeEndDate, dirtyComparedRangeStartDate, dirtyComparedRangeEndDate ) {
  var initialStartTime = parse(dirtyInitialRangeStartDate).getTime()
  var initialEndTime = parse(dirtyInitialRangeEndDate).getTime()
  var comparedStartTime = parse(dirtyComparedRangeStartDate).getTime()
  var comparedEndTime = parse(dirtyComparedRangeEndDate).getTime()

  if (initialStartTime > initialEndTime || comparedStartTime > comparedEndTime) {
    throw new Error('The start of the range cannot be after the end of the range')
  }

  return initialStartTime < comparedEndTime && comparedStartTime < initialEndTime
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.closestIndexTo"></a>[function <span class="apidocSignatureSpan">date-fns.</span>closestIndexTo (dirtyDateToCompare, dirtyDatesArray)](#apidoc.element.date-fns.closestIndexTo)
- description and source-code
```javascript
function closestIndexTo(dirtyDateToCompare, dirtyDatesArray) {
  if (!(dirtyDatesArray instanceof Array)) {
    throw new TypeError(toString.call(dirtyDatesArray) + ' is not an instance of Array')
  }

  var dateToCompare = parse(dirtyDateToCompare)
  var timeToCompare = dateToCompare.getTime()

  var result
  var minDistance

  dirtyDatesArray.forEach(function (dirtyDate, index) {
    var currentDate = parse(dirtyDate)
    var distance = Math.abs(timeToCompare - currentDate.getTime())
    if (result === undefined || distance < minDistance) {
      result = index
      minDistance = distance
    }
  })

  return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.closestTo"></a>[function <span class="apidocSignatureSpan">date-fns.</span>closestTo (dirtyDateToCompare, dirtyDatesArray)](#apidoc.element.date-fns.closestTo)
- description and source-code
```javascript
function closestTo(dirtyDateToCompare, dirtyDatesArray) {
  if (!(dirtyDatesArray instanceof Array)) {
    throw new TypeError(toString.call(dirtyDatesArray) + ' is not an instance of Array')
  }

  var dateToCompare = parse(dirtyDateToCompare)
  var timeToCompare = dateToCompare.getTime()

  var result
  var minDistance

  dirtyDatesArray.forEach(function (dirtyDate) {
    var currentDate = parse(dirtyDate)
    var distance = Math.abs(timeToCompare - currentDate.getTime())
    if (result === undefined || distance < minDistance) {
      result = currentDate
      minDistance = distance
    }
  })

  return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.compareAsc"></a>[function <span class="apidocSignatureSpan">date-fns.</span>compareAsc (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.compareAsc)
- description and source-code
```javascript
function compareAsc(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var timeLeft = dateLeft.getTime()
  var dateRight = parse(dirtyDateRight)
  var timeRight = dateRight.getTime()

  if (timeLeft < timeRight) {
    return -1
  } else if (timeLeft > timeRight) {
    return 1
  } else {
    return 0
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.compareDesc"></a>[function <span class="apidocSignatureSpan">date-fns.</span>compareDesc (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.compareDesc)
- description and source-code
```javascript
function compareDesc(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var timeLeft = dateLeft.getTime()
  var dateRight = parse(dirtyDateRight)
  var timeRight = dateRight.getTime()

  if (timeLeft > timeRight) {
    return -1
  } else if (timeLeft < timeRight) {
    return 1
  } else {
    return 0
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarDays"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarDays (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarDays)
- description and source-code
```javascript
function differenceInCalendarDays(dirtyDateLeft, dirtyDateRight) {
  var startOfDayLeft = startOfDay(dirtyDateLeft)
  var startOfDayRight = startOfDay(dirtyDateRight)

  var timestampLeft = startOfDayLeft.getTime() -
    startOfDayLeft.getTimezoneOffset() * MILLISECONDS_IN_MINUTE
  var timestampRight = startOfDayRight.getTime() -
    startOfDayRight.getTimezoneOffset() * MILLISECONDS_IN_MINUTE

  // Round the number of days to the nearest integer
  // because the number of milliseconds in a day is not constant
  // (e.g. it's different in the day of the daylight saving time clock shift)
  return Math.round((timestampLeft - timestampRight) / MILLISECONDS_IN_DAY)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarISOWeeks"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarISOWeeks (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarISOWeeks)
- description and source-code
```javascript
function differenceInCalendarISOWeeks(dirtyDateLeft, dirtyDateRight) {
  var startOfISOWeekLeft = startOfISOWeek(dirtyDateLeft)
  var startOfISOWeekRight = startOfISOWeek(dirtyDateRight)

  var timestampLeft = startOfISOWeekLeft.getTime() -
    startOfISOWeekLeft.getTimezoneOffset() * MILLISECONDS_IN_MINUTE
  var timestampRight = startOfISOWeekRight.getTime() -
    startOfISOWeekRight.getTimezoneOffset() * MILLISECONDS_IN_MINUTE

  // Round the number of days to the nearest integer
  // because the number of milliseconds in a week is not constant
  // (e.g. it's different in the week of the daylight saving time clock shift)
  return Math.round((timestampLeft - timestampRight) / MILLISECONDS_IN_WEEK)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarISOYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarISOYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarISOYears)
- description and source-code
```javascript
function differenceInCalendarISOYears(dirtyDateLeft, dirtyDateRight) {
  return getISOYear(dirtyDateLeft) - getISOYear(dirtyDateRight)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarMonths"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarMonths (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarMonths)
- description and source-code
```javascript
function differenceInCalendarMonths(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  var yearDiff = dateLeft.getFullYear() - dateRight.getFullYear()
  var monthDiff = dateLeft.getMonth() - dateRight.getMonth()

  return yearDiff * 12 + monthDiff
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarQuarters"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarQuarters (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarQuarters)
- description and source-code
```javascript
function differenceInCalendarQuarters(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  var yearDiff = dateLeft.getFullYear() - dateRight.getFullYear()
  var quarterDiff = getQuarter(dateLeft) - getQuarter(dateRight)

  return yearDiff * 4 + quarterDiff
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarWeeks"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarWeeks (dirtyDateLeft, dirtyDateRight, dirtyOptions)](#apidoc.element.date-fns.differenceInCalendarWeeks)
- description and source-code
```javascript
function differenceInCalendarWeeks(dirtyDateLeft, dirtyDateRight, dirtyOptions) {
  var startOfWeekLeft = startOfWeek(dirtyDateLeft, dirtyOptions)
  var startOfWeekRight = startOfWeek(dirtyDateRight, dirtyOptions)

  var timestampLeft = startOfWeekLeft.getTime() -
    startOfWeekLeft.getTimezoneOffset() * MILLISECONDS_IN_MINUTE
  var timestampRight = startOfWeekRight.getTime() -
    startOfWeekRight.getTimezoneOffset() * MILLISECONDS_IN_MINUTE

  // Round the number of days to the nearest integer
  // because the number of milliseconds in a week is not constant
  // (e.g. it's different in the week of the daylight saving time clock shift)
  return Math.round((timestampLeft - timestampRight) / MILLISECONDS_IN_WEEK)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInCalendarYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInCalendarYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInCalendarYears)
- description and source-code
```javascript
function differenceInCalendarYears(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  return dateLeft.getFullYear() - dateRight.getFullYear()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInDays"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInDays (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInDays)
- description and source-code
```javascript
function differenceInDays(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  var sign = compareAsc(dateLeft, dateRight)
  var difference = Math.abs(differenceInCalendarDays(dateLeft, dateRight))
  dateLeft.setDate(dateLeft.getDate() - sign * difference)

  // Math.abs(diff in full days - diff in calendar days) === 1 if last calendar day is not full
  // If so, result must be decreased by 1 in absolute value
  var isLastDayNotFull = compareAsc(dateLeft, dateRight) === -sign
  return sign * (difference - isLastDayNotFull)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInHours"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInHours (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInHours)
- description and source-code
```javascript
function differenceInHours(dirtyDateLeft, dirtyDateRight) {
  var diff = differenceInMilliseconds(dirtyDateLeft, dirtyDateRight) / MILLISECONDS_IN_HOUR
  return diff > 0 ? Math.floor(diff) : Math.ceil(diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInISOYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInISOYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInISOYears)
- description and source-code
```javascript
function differenceInISOYears(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  var sign = compareAsc(dateLeft, dateRight)
  var difference = Math.abs(differenceInCalendarISOYears(dateLeft, dateRight))
  dateLeft = subISOYears(dateLeft, sign * difference)

  // Math.abs(diff in full ISO years - diff in calendar ISO years) === 1
  // if last calendar ISO year is not full
  // If so, result must be decreased by 1 in absolute value
  var isLastISOYearNotFull = compareAsc(dateLeft, dateRight) === -sign
  return sign * (difference - isLastISOYearNotFull)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInMilliseconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInMilliseconds (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInMilliseconds)
- description and source-code
```javascript
function differenceInMilliseconds(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)
  return dateLeft.getTime() - dateRight.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInMinutes"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInMinutes (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInMinutes)
- description and source-code
```javascript
function differenceInMinutes(dirtyDateLeft, dirtyDateRight) {
  var diff = differenceInMilliseconds(dirtyDateLeft, dirtyDateRight) / MILLISECONDS_IN_MINUTE
  return diff > 0 ? Math.floor(diff) : Math.ceil(diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInMonths"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInMonths (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInMonths)
- description and source-code
```javascript
function differenceInMonths(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  var sign = compareAsc(dateLeft, dateRight)
  var difference = Math.abs(differenceInCalendarMonths(dateLeft, dateRight))
  dateLeft.setMonth(dateLeft.getMonth() - sign * difference)

  // Math.abs(diff in full months - diff in calendar months) === 1 if last calendar month is not full
  // If so, result must be decreased by 1 in absolute value
  var isLastMonthNotFull = compareAsc(dateLeft, dateRight) === -sign
  return sign * (difference - isLastMonthNotFull)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInQuarters"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInQuarters (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInQuarters)
- description and source-code
```javascript
function differenceInQuarters(dirtyDateLeft, dirtyDateRight) {
  var diff = differenceInMonths(dirtyDateLeft, dirtyDateRight) / 3
  return diff > 0 ? Math.floor(diff) : Math.ceil(diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInSeconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInSeconds (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInSeconds)
- description and source-code
```javascript
function differenceInSeconds(dirtyDateLeft, dirtyDateRight) {
  var diff = differenceInMilliseconds(dirtyDateLeft, dirtyDateRight) / 1000
  return diff > 0 ? Math.floor(diff) : Math.ceil(diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInWeeks"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInWeeks (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInWeeks)
- description and source-code
```javascript
function differenceInWeeks(dirtyDateLeft, dirtyDateRight) {
  var diff = differenceInDays(dirtyDateLeft, dirtyDateRight) / 7
  return diff > 0 ? Math.floor(diff) : Math.ceil(diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.differenceInYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>differenceInYears (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.differenceInYears)
- description and source-code
```javascript
function differenceInYears(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)

  var sign = compareAsc(dateLeft, dateRight)
  var difference = Math.abs(differenceInCalendarYears(dateLeft, dateRight))
  dateLeft.setFullYear(dateLeft.getFullYear() - sign * difference)

  // Math.abs(diff in full years - diff in calendar years) === 1 if last calendar year is not full
  // If so, result must be decreased by 1 in absolute value
  var isLastYearNotFull = compareAsc(dateLeft, dateRight) === -sign
  return sign * (difference - isLastYearNotFull)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.distanceInWords"></a>[function <span class="apidocSignatureSpan">date-fns.</span>distanceInWords (dirtyDateToCompare, dirtyDate, dirtyOptions)](#apidoc.element.date-fns.distanceInWords)
- description and source-code
```javascript
function distanceInWords(dirtyDateToCompare, dirtyDate, dirtyOptions) {
  var options = dirtyOptions || {}

  var comparison = compareDesc(dirtyDateToCompare, dirtyDate)

  var locale = options.locale
  var localize = enLocale.distanceInWords.localize
  if (locale && locale.distanceInWords && locale.distanceInWords.localize) {
    localize = locale.distanceInWords.localize
  }

  var localizeOptions = {
    addSuffix: Boolean(options.addSuffix),
    comparison: comparison
  }

  var dateLeft, dateRight
  if (comparison > 0) {
    dateLeft = parse(dirtyDateToCompare)
    dateRight = parse(dirtyDate)
  } else {
    dateLeft = parse(dirtyDate)
    dateRight = parse(dirtyDateToCompare)
  }

  var seconds = differenceInSeconds(dateRight, dateLeft)
  var offset = dateRight.getTimezoneOffset() - dateLeft.getTimezoneOffset()
  var minutes = Math.round(seconds / 60) - offset
  var months

  // 0 up to 2 mins
  if (minutes < 2) {
    if (options.includeSeconds) {
      if (seconds < 5) {
        return localize('lessThanXSeconds', 5, localizeOptions)
      } else if (seconds < 10) {
        return localize('lessThanXSeconds', 10, localizeOptions)
      } else if (seconds < 20) {
        return localize('lessThanXSeconds', 20, localizeOptions)
      } else if (seconds < 40) {
        return localize('halfAMinute', null, localizeOptions)
      } else if (seconds < 60) {
        return localize('lessThanXMinutes', 1, localizeOptions)
      } else {
        return localize('xMinutes', 1, localizeOptions)
      }
    } else {
      if (minutes === 0) {
        return localize('lessThanXMinutes', 1, localizeOptions)
      } else {
        return localize('xMinutes', minutes, localizeOptions)
      }
    }

  // 2 mins up to 0.75 hrs
  } else if (minutes < 45) {
    return localize('xMinutes', minutes, localizeOptions)

  // 0.75 hrs up to 1.5 hrs
  } else if (minutes < 90) {
    return localize('aboutXHours', 1, localizeOptions)

  // 1.5 hrs up to 24 hrs
  } else if (minutes < MINUTES_IN_DAY) {
    var hours = Math.round(minutes / 60)
    return localize('aboutXHours', hours, localizeOptions)

  // 1 day up to 1.75 days
  } else if (minutes < MINUTES_IN_ALMOST_TWO_DAYS) {
    return localize('xDays', 1, localizeOptions)

  // 1.75 days up to 30 days
  } else if (minutes < MINUTES_IN_MONTH) {
    var days = Math.round(minutes / MINUTES_IN_DAY)
    return localize('xDays', days, localizeOptions)

  // 1 month up to 2 months
  } else if (minutes < MINUTES_IN_TWO_MONTHS) {
    months = Math.round(minutes / MINUTES_IN_MONTH)
    return localize('aboutXMonths', months, localizeOptions)
  }

  months = differenceInMonths(dateRight, dateLeft)

  // 2 months up to 12 months
  if (months < 12) {
    var nearestMonth = Math.round(minutes / MINUTES_IN_MONTH)
    return localize('xMonths', nearestMonth, localizeOptions)

  // 1 year up to max Date
  } else {
    var monthsSinceStartOfYear = months % 12
    var years = Math.floor(months / 12)

    // N years up to 1 years 3 months
    if (monthsSinceStartOfYear < 3) {
      return localize('aboutXYears', years, localizeOptions)

    // N years 3 months up to N years 9 months
    } else if (monthsSinceStartOfYear < 9) {
      return localize('overXYears', years, localizeOptions)

    // N years 9 months up to N year 12 months
    } else {
      return localize('almostXYears', years + 1, localizeOptions)
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.distanceInWordsStrict"></a>[function <span class="apidocSignatureSpan">date-fns.</span>distanceInWordsStrict (dirtyDateToCompare, dirtyDate, dirtyOptions)](#apidoc.element.date-fns.distanceInWordsStrict)
- description and source-code
```javascript
function distanceInWordsStrict(dirtyDateToCompare, dirtyDate, dirtyOptions) {
  var options = dirtyOptions || {}

  var comparison = compareDesc(dirtyDateToCompare, dirtyDate)

  var locale = options.locale
  var localize = enLocale.distanceInWords.localize
  if (locale && locale.distanceInWords && locale.distanceInWords.localize) {
    localize = locale.distanceInWords.localize
  }

  var localizeOptions = {
    addSuffix: Boolean(options.addSuffix),
    comparison: comparison
  }

  var dateLeft, dateRight
  if (comparison > 0) {
    dateLeft = parse(dirtyDateToCompare)
    dateRight = parse(dirtyDate)
  } else {
    dateLeft = parse(dirtyDate)
    dateRight = parse(dirtyDateToCompare)
  }

  var unit
  var mathPartial = Math[options.partialMethod ? String(options.partialMethod) : 'floor']
  var seconds = differenceInSeconds(dateRight, dateLeft)
  var offset = dateRight.getTimezoneOffset() - dateLeft.getTimezoneOffset()
  var minutes = mathPartial(seconds / 60) - offset
  var hours, days, months, years

  if (options.unit) {
    unit = String(options.unit)
  } else {
    if (minutes < 1) {
      unit = 's'
    } else if (minutes < 60) {
      unit = 'm'
    } else if (minutes < MINUTES_IN_DAY) {
      unit = 'h'
    } else if (minutes < MINUTES_IN_MONTH) {
      unit = 'd'
    } else if (minutes < MINUTES_IN_YEAR) {
      unit = 'M'
    } else {
      unit = 'Y'
    }
  }

  // 0 up to 60 seconds
  if (unit === 's') {
    return localize('xSeconds', seconds, localizeOptions)

  // 1 up to 60 mins
  } else if (unit === 'm') {
    return localize('xMinutes', minutes, localizeOptions)

  // 1 up to 24 hours
  } else if (unit === 'h') {
    hours = mathPartial(minutes / 60)
    return localize('xHours', hours, localizeOptions)

  // 1 up to 30 days
  } else if (unit === 'd') {
    days = mathPartial(minutes / MINUTES_IN_DAY)
    return localize('xDays', days, localizeOptions)

  // 1 up to 12 months
  } else if (unit === 'M') {
    months = mathPartial(minutes / MINUTES_IN_MONTH)
    return localize('xMonths', months, localizeOptions)

  // 1 year up to max Date
  } else if (unit === 'Y') {
    years = mathPartial(minutes / MINUTES_IN_YEAR)
    return localize('xYears', years, localizeOptions)
  }

  throw new Error('Unknown unit: ' + unit)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.distanceInWordsToNow"></a>[function <span class="apidocSignatureSpan">date-fns.</span>distanceInWordsToNow (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.distanceInWordsToNow)
- description and source-code
```javascript
function distanceInWordsToNow(dirtyDate, dirtyOptions) {
  return distanceInWords(Date.now(), dirtyDate, dirtyOptions)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.eachDay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>eachDay (dirtyStartDate, dirtyEndDate)](#apidoc.element.date-fns.eachDay)
- description and source-code
```javascript
function eachDay(dirtyStartDate, dirtyEndDate) {
  var startDate = parse(dirtyStartDate)
  var endDate = parse(dirtyEndDate)

  var endTime = endDate.getTime()

  if (startDate.getTime() > endTime) {
    throw new Error('The first date cannot be after the second date')
  }

  var dates = []

  var currentDate = startDate
  currentDate.setHours(0, 0, 0, 0)

  while (currentDate.getTime() <= endTime) {
    dates.push(parse(currentDate))
    currentDate.setDate(currentDate.getDate() + 1)
  }

  return dates
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfDay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfDay (dirtyDate)](#apidoc.element.date-fns.endOfDay)
- description and source-code
```javascript
function endOfDay(dirtyDate) {
  var date = parse(dirtyDate)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfHour"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfHour (dirtyDate)](#apidoc.element.date-fns.endOfHour)
- description and source-code
```javascript
function endOfHour(dirtyDate) {
  var date = parse(dirtyDate)
  date.setMinutes(59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfISOWeek (dirtyDate)](#apidoc.element.date-fns.endOfISOWeek)
- description and source-code
```javascript
function endOfISOWeek(dirtyDate) {
  return endOfWeek(dirtyDate, {weekStartsOn: 1})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfISOYear (dirtyDate)](#apidoc.element.date-fns.endOfISOYear)
- description and source-code
```javascript
function endOfISOYear(dirtyDate) {
  var year = getISOYear(dirtyDate)
  var fourthOfJanuaryOfNextYear = new Date(0)
  fourthOfJanuaryOfNextYear.setFullYear(year + 1, 0, 4)
  fourthOfJanuaryOfNextYear.setHours(0, 0, 0, 0)
  var date = startOfISOWeek(fourthOfJanuaryOfNextYear)
  date.setMilliseconds(date.getMilliseconds() - 1)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfMinute"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfMinute (dirtyDate)](#apidoc.element.date-fns.endOfMinute)
- description and source-code
```javascript
function endOfMinute(dirtyDate) {
  var date = parse(dirtyDate)
  date.setSeconds(59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfMonth (dirtyDate)](#apidoc.element.date-fns.endOfMonth)
- description and source-code
```javascript
function endOfMonth(dirtyDate) {
  var date = parse(dirtyDate)
  var month = date.getMonth()
  date.setFullYear(date.getFullYear(), month + 1, 0)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfQuarter (dirtyDate)](#apidoc.element.date-fns.endOfQuarter)
- description and source-code
```javascript
function endOfQuarter(dirtyDate) {
  var date = parse(dirtyDate)
  var currentMonth = date.getMonth()
  var month = currentMonth - currentMonth % 3 + 3
  date.setMonth(month, 0)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfSecond"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfSecond (dirtyDate)](#apidoc.element.date-fns.endOfSecond)
- description and source-code
```javascript
function endOfSecond(dirtyDate) {
  var date = parse(dirtyDate)
  date.setMilliseconds(999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfToday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfToday ()](#apidoc.element.date-fns.endOfToday)
- description and source-code
```javascript
function endOfToday() {
  return endOfDay(new Date())
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfTomorrow"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfTomorrow ()](#apidoc.element.date-fns.endOfTomorrow)
- description and source-code
```javascript
function endOfTomorrow() {
  var now = new Date()
  var year = now.getFullYear()
  var month = now.getMonth()
  var day = now.getDate()

  var date = new Date(0)
  date.setFullYear(year, month, day + 1)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.endOfWeek)
- description and source-code
```javascript
function endOfWeek(dirtyDate, dirtyOptions) {
  var weekStartsOn = dirtyOptions ? (Number(dirtyOptions.weekStartsOn) || 0) : 0

  var date = parse(dirtyDate)
  var day = date.getDay()
  var diff = (day < weekStartsOn ? -7 : 0) + 6 - (day - weekStartsOn)

  date.setDate(date.getDate() + diff)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfYear (dirtyDate)](#apidoc.element.date-fns.endOfYear)
- description and source-code
```javascript
function endOfYear(dirtyDate) {
  var date = parse(dirtyDate)
  var year = date.getFullYear()
  date.setFullYear(year + 1, 0, 0)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.endOfYesterday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>endOfYesterday ()](#apidoc.element.date-fns.endOfYesterday)
- description and source-code
```javascript
function endOfYesterday() {
  var now = new Date()
  var year = now.getFullYear()
  var month = now.getMonth()
  var day = now.getDate()

  var date = new Date(0)
  date.setFullYear(year, month, day - 1)
  date.setHours(23, 59, 59, 999)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.format"></a>[function <span class="apidocSignatureSpan">date-fns.</span>format (dirtyDate, dirtyFormatStr, dirtyOptions)](#apidoc.element.date-fns.format)
- description and source-code
```javascript
function format(dirtyDate, dirtyFormatStr, dirtyOptions) {
  var formatStr = dirtyFormatStr ? String(dirtyFormatStr) : 'YYYY-MM-DDTHH:mm:ss.SSSZ'
  var options = dirtyOptions || {}

  var locale = options.locale
  var localeFormatters = enLocale.format.formatters
  var formattingTokensRegExp = enLocale.format.formattingTokensRegExp
  if (locale && locale.format && locale.format.formatters) {
    localeFormatters = locale.format.formatters

    if (locale.format.formattingTokensRegExp) {
      formattingTokensRegExp = locale.format.formattingTokensRegExp
    }
  }

  var date = parse(dirtyDate)

  if (!isValid(date)) {
    return 'Invalid Date'
  }

  var formatFn = buildFormatFn(formatStr, localeFormatters, formattingTokensRegExp)

  return formatFn(date)
}
```
- example usage
```shell
...
**date-fns** provides the most comprehensive, yet simple and consistent toolset
for manipulating **JavaScript dates** in **a browser** & **Node.js**.

**date-fns** is like [lodash](https://lodash.com) for dates. It has
[**140+ functions** for all occasions](https://date-fns.org/docs/).

'''js
dateFns.format(new Date(2014, 1, 11), 'MM/DD/YYYY')
//=> '02/11/2014'

var dates = [new Date(1995, 6, 2), new Date(1987, 1, 11), new Date(1989, 6, 10)]
dates.sort(dateFns.compareAsc)
//=> [
//   Wed Feb 11 1987 00:00:00,
//   Mon Jul 10 1989 00:00:00,
...
```

#### <a name="apidoc.element.date-fns.getDate"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getDate (dirtyDate)](#apidoc.element.date-fns.getDate)
- description and source-code
```javascript
function getDate(dirtyDate) {
  var date = parse(dirtyDate)
  var dayOfMonth = date.getDate()
  return dayOfMonth
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getDay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getDay (dirtyDate)](#apidoc.element.date-fns.getDay)
- description and source-code
```javascript
function getDay(dirtyDate) {
  var date = parse(dirtyDate)
  var day = date.getDay()
  return day
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getDayOfYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getDayOfYear (dirtyDate)](#apidoc.element.date-fns.getDayOfYear)
- description and source-code
```javascript
function getDayOfYear(dirtyDate) {
  var date = parse(dirtyDate)
  var diff = differenceInCalendarDays(date, startOfYear(date))
  var dayOfYear = diff + 1
  return dayOfYear
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getDaysInMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getDaysInMonth (dirtyDate)](#apidoc.element.date-fns.getDaysInMonth)
- description and source-code
```javascript
function getDaysInMonth(dirtyDate) {
  var date = parse(dirtyDate)
  var year = date.getFullYear()
  var monthIndex = date.getMonth()
  var lastDayOfMonth = new Date(0)
  lastDayOfMonth.setFullYear(year, monthIndex + 1, 0)
  lastDayOfMonth.setHours(0, 0, 0, 0)
  return lastDayOfMonth.getDate()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getDaysInYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getDaysInYear (dirtyDate)](#apidoc.element.date-fns.getDaysInYear)
- description and source-code
```javascript
function getDaysInYear(dirtyDate) {
  return isLeapYear(dirtyDate) ? 366 : 365
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getHours"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getHours (dirtyDate)](#apidoc.element.date-fns.getHours)
- description and source-code
```javascript
function getHours(dirtyDate) {
  var date = parse(dirtyDate)
  var hours = date.getHours()
  return hours
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getISODay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getISODay (dirtyDate)](#apidoc.element.date-fns.getISODay)
- description and source-code
```javascript
function getISODay(dirtyDate) {
  var date = parse(dirtyDate)
  var day = date.getDay()

  if (day === 0) {
    day = 7
  }

  return day
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getISOWeek (dirtyDate)](#apidoc.element.date-fns.getISOWeek)
- description and source-code
```javascript
function getISOWeek(dirtyDate) {
  var date = parse(dirtyDate)
  var diff = startOfISOWeek(date).getTime() - startOfISOYear(date).getTime()

  // Round the number of days to the nearest integer
  // because the number of milliseconds in a week is not constant
  // (e.g. it's different in the week of the daylight saving time clock shift)
  return Math.round(diff / MILLISECONDS_IN_WEEK) + 1
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getISOWeeksInYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getISOWeeksInYear (dirtyDate)](#apidoc.element.date-fns.getISOWeeksInYear)
- description and source-code
```javascript
function getISOWeeksInYear(dirtyDate) {
  var thisYear = startOfISOYear(dirtyDate)
  var nextYear = startOfISOYear(addWeeks(thisYear, 60))
  var diff = nextYear.valueOf() - thisYear.valueOf()
  // Round the number of weeks to the nearest integer
  // because the number of milliseconds in a week is not constant
  // (e.g. it's different in the week of the daylight saving time clock shift)
  return Math.round(diff / MILLISECONDS_IN_WEEK)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getISOYear (dirtyDate)](#apidoc.element.date-fns.getISOYear)
- description and source-code
```javascript
function getISOYear(dirtyDate) {
  var date = parse(dirtyDate)
  var year = date.getFullYear()

  var fourthOfJanuaryOfNextYear = new Date(0)
  fourthOfJanuaryOfNextYear.setFullYear(year + 1, 0, 4)
  fourthOfJanuaryOfNextYear.setHours(0, 0, 0, 0)
  var startOfNextYear = startOfISOWeek(fourthOfJanuaryOfNextYear)

  var fourthOfJanuaryOfThisYear = new Date(0)
  fourthOfJanuaryOfThisYear.setFullYear(year, 0, 4)
  fourthOfJanuaryOfThisYear.setHours(0, 0, 0, 0)
  var startOfThisYear = startOfISOWeek(fourthOfJanuaryOfThisYear)

  if (date.getTime() >= startOfNextYear.getTime()) {
    return year + 1
  } else if (date.getTime() >= startOfThisYear.getTime()) {
    return year
  } else {
    return year - 1
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getMilliseconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getMilliseconds (dirtyDate)](#apidoc.element.date-fns.getMilliseconds)
- description and source-code
```javascript
function getMilliseconds(dirtyDate) {
  var date = parse(dirtyDate)
  var milliseconds = date.getMilliseconds()
  return milliseconds
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getMinutes"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getMinutes (dirtyDate)](#apidoc.element.date-fns.getMinutes)
- description and source-code
```javascript
function getMinutes(dirtyDate) {
  var date = parse(dirtyDate)
  var minutes = date.getMinutes()
  return minutes
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getMonth (dirtyDate)](#apidoc.element.date-fns.getMonth)
- description and source-code
```javascript
function getMonth(dirtyDate) {
  var date = parse(dirtyDate)
  var month = date.getMonth()
  return month
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getOverlappingDaysInRanges"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getOverlappingDaysInRanges (dirtyInitialRangeStartDate, dirtyInitialRangeEndDate, dirtyComparedRangeStartDate, dirtyComparedRangeEndDate )](#apidoc.element.date-fns.getOverlappingDaysInRanges)
- description and source-code
```javascript
function getOverlappingDaysInRanges(dirtyInitialRangeStartDate, dirtyInitialRangeEndDate, dirtyComparedRangeStartDate, dirtyComparedRangeEndDate ) {
  var initialStartTime = parse(dirtyInitialRangeStartDate).getTime()
  var initialEndTime = parse(dirtyInitialRangeEndDate).getTime()
  var comparedStartTime = parse(dirtyComparedRangeStartDate).getTime()
  var comparedEndTime = parse(dirtyComparedRangeEndDate).getTime()

  if (initialStartTime > initialEndTime || comparedStartTime > comparedEndTime) {
    throw new Error('The start of the range cannot be after the end of the range')
  }

  var isOverlapping = initialStartTime < comparedEndTime && comparedStartTime < initialEndTime

  if (!isOverlapping) {
    return 0
  }

  var overlapStartDate = comparedStartTime < initialStartTime
    ? initialStartTime
    : comparedStartTime

  var overlapEndDate = comparedEndTime > initialEndTime
    ? initialEndTime
    : comparedEndTime

  var differenceInMs = overlapEndDate - overlapStartDate

  return Math.ceil(differenceInMs / MILLISECONDS_IN_DAY)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getQuarter (dirtyDate)](#apidoc.element.date-fns.getQuarter)
- description and source-code
```javascript
function getQuarter(dirtyDate) {
  var date = parse(dirtyDate)
  var quarter = Math.floor(date.getMonth() / 3) + 1
  return quarter
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getSeconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getSeconds (dirtyDate)](#apidoc.element.date-fns.getSeconds)
- description and source-code
```javascript
function getSeconds(dirtyDate) {
  var date = parse(dirtyDate)
  var seconds = date.getSeconds()
  return seconds
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getTime"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getTime (dirtyDate)](#apidoc.element.date-fns.getTime)
- description and source-code
```javascript
function getTime(dirtyDate) {
  var date = parse(dirtyDate)
  var timestamp = date.getTime()
  return timestamp
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.getYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>getYear (dirtyDate)](#apidoc.element.date-fns.getYear)
- description and source-code
```javascript
function getYear(dirtyDate) {
  var date = parse(dirtyDate)
  var year = date.getFullYear()
  return year
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isAfter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isAfter (dirtyDate, dirtyDateToCompare)](#apidoc.element.date-fns.isAfter)
- description and source-code
```javascript
function isAfter(dirtyDate, dirtyDateToCompare) {
  var date = parse(dirtyDate)
  var dateToCompare = parse(dirtyDateToCompare)
  return date.getTime() > dateToCompare.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isBefore"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isBefore (dirtyDate, dirtyDateToCompare)](#apidoc.element.date-fns.isBefore)
- description and source-code
```javascript
function isBefore(dirtyDate, dirtyDateToCompare) {
  var date = parse(dirtyDate)
  var dateToCompare = parse(dirtyDateToCompare)
  return date.getTime() < dateToCompare.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isDate"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isDate (argument)](#apidoc.element.date-fns.isDate)
- description and source-code
```javascript
function isDate(argument) {
  return argument instanceof Date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isEqual"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isEqual (dirtyLeftDate, dirtyRightDate)](#apidoc.element.date-fns.isEqual)
- description and source-code
```javascript
function isEqual(dirtyLeftDate, dirtyRightDate) {
  var dateLeft = parse(dirtyLeftDate)
  var dateRight = parse(dirtyRightDate)
  return dateLeft.getTime() === dateRight.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isFirstDayOfMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isFirstDayOfMonth (dirtyDate)](#apidoc.element.date-fns.isFirstDayOfMonth)
- description and source-code
```javascript
function isFirstDayOfMonth(dirtyDate) {
  return parse(dirtyDate).getDate() === 1
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isFriday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isFriday (dirtyDate)](#apidoc.element.date-fns.isFriday)
- description and source-code
```javascript
function isFriday(dirtyDate) {
  return parse(dirtyDate).getDay() === 5
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isFuture"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isFuture (dirtyDate)](#apidoc.element.date-fns.isFuture)
- description and source-code
```javascript
function isFuture(dirtyDate) {
  return parse(dirtyDate).getTime() > new Date().getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isLastDayOfMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isLastDayOfMonth (dirtyDate)](#apidoc.element.date-fns.isLastDayOfMonth)
- description and source-code
```javascript
function isLastDayOfMonth(dirtyDate) {
  var date = parse(dirtyDate)
  return endOfDay(date).getTime() === endOfMonth(date).getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isLeapYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isLeapYear (dirtyDate)](#apidoc.element.date-fns.isLeapYear)
- description and source-code
```javascript
function isLeapYear(dirtyDate) {
  var date = parse(dirtyDate)
  var year = date.getFullYear()
  return year % 400 === 0 || year % 4 === 0 && year % 100 !== 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isMonday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isMonday (dirtyDate)](#apidoc.element.date-fns.isMonday)
- description and source-code
```javascript
function isMonday(dirtyDate) {
  return parse(dirtyDate).getDay() === 1
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isPast"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isPast (dirtyDate)](#apidoc.element.date-fns.isPast)
- description and source-code
```javascript
function isPast(dirtyDate) {
  return parse(dirtyDate).getTime() < new Date().getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameDay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameDay (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameDay)
- description and source-code
```javascript
function isSameDay(dirtyDateLeft, dirtyDateRight) {
  var dateLeftStartOfDay = startOfDay(dirtyDateLeft)
  var dateRightStartOfDay = startOfDay(dirtyDateRight)

  return dateLeftStartOfDay.getTime() === dateRightStartOfDay.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameHour"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameHour (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameHour)
- description and source-code
```javascript
function isSameHour(dirtyDateLeft, dirtyDateRight) {
  var dateLeftStartOfHour = startOfHour(dirtyDateLeft)
  var dateRightStartOfHour = startOfHour(dirtyDateRight)

  return dateLeftStartOfHour.getTime() === dateRightStartOfHour.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameISOWeek (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameISOWeek)
- description and source-code
```javascript
function isSameISOWeek(dirtyDateLeft, dirtyDateRight) {
  return isSameWeek(dirtyDateLeft, dirtyDateRight, {weekStartsOn: 1})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameISOYear (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameISOYear)
- description and source-code
```javascript
function isSameISOYear(dirtyDateLeft, dirtyDateRight) {
  var dateLeftStartOfYear = startOfISOYear(dirtyDateLeft)
  var dateRightStartOfYear = startOfISOYear(dirtyDateRight)

  return dateLeftStartOfYear.getTime() === dateRightStartOfYear.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameMinute"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameMinute (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameMinute)
- description and source-code
```javascript
function isSameMinute(dirtyDateLeft, dirtyDateRight) {
  var dateLeftStartOfMinute = startOfMinute(dirtyDateLeft)
  var dateRightStartOfMinute = startOfMinute(dirtyDateRight)

  return dateLeftStartOfMinute.getTime() === dateRightStartOfMinute.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameMonth (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameMonth)
- description and source-code
```javascript
function isSameMonth(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)
  return dateLeft.getFullYear() === dateRight.getFullYear() &&
    dateLeft.getMonth() === dateRight.getMonth()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameQuarter (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameQuarter)
- description and source-code
```javascript
function isSameQuarter(dirtyDateLeft, dirtyDateRight) {
  var dateLeftStartOfQuarter = startOfQuarter(dirtyDateLeft)
  var dateRightStartOfQuarter = startOfQuarter(dirtyDateRight)

  return dateLeftStartOfQuarter.getTime() === dateRightStartOfQuarter.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameSecond"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameSecond (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameSecond)
- description and source-code
```javascript
function isSameSecond(dirtyDateLeft, dirtyDateRight) {
  var dateLeftStartOfSecond = startOfSecond(dirtyDateLeft)
  var dateRightStartOfSecond = startOfSecond(dirtyDateRight)

  return dateLeftStartOfSecond.getTime() === dateRightStartOfSecond.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameWeek (dirtyDateLeft, dirtyDateRight, dirtyOptions)](#apidoc.element.date-fns.isSameWeek)
- description and source-code
```javascript
function isSameWeek(dirtyDateLeft, dirtyDateRight, dirtyOptions) {
  var dateLeftStartOfWeek = startOfWeek(dirtyDateLeft, dirtyOptions)
  var dateRightStartOfWeek = startOfWeek(dirtyDateRight, dirtyOptions)

  return dateLeftStartOfWeek.getTime() === dateRightStartOfWeek.getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSameYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSameYear (dirtyDateLeft, dirtyDateRight)](#apidoc.element.date-fns.isSameYear)
- description and source-code
```javascript
function isSameYear(dirtyDateLeft, dirtyDateRight) {
  var dateLeft = parse(dirtyDateLeft)
  var dateRight = parse(dirtyDateRight)
  return dateLeft.getFullYear() === dateRight.getFullYear()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSaturday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSaturday (dirtyDate)](#apidoc.element.date-fns.isSaturday)
- description and source-code
```javascript
function isSaturday(dirtyDate) {
  return parse(dirtyDate).getDay() === 6
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isSunday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isSunday (dirtyDate)](#apidoc.element.date-fns.isSunday)
- description and source-code
```javascript
function isSunday(dirtyDate) {
  return parse(dirtyDate).getDay() === 0
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisHour"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisHour (dirtyDate)](#apidoc.element.date-fns.isThisHour)
- description and source-code
```javascript
function isThisHour(dirtyDate) {
  return isSameHour(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisISOWeek (dirtyDate)](#apidoc.element.date-fns.isThisISOWeek)
- description and source-code
```javascript
function isThisISOWeek(dirtyDate) {
  return isSameISOWeek(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisISOYear (dirtyDate)](#apidoc.element.date-fns.isThisISOYear)
- description and source-code
```javascript
function isThisISOYear(dirtyDate) {
  return isSameISOYear(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisMinute"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisMinute (dirtyDate)](#apidoc.element.date-fns.isThisMinute)
- description and source-code
```javascript
function isThisMinute(dirtyDate) {
  return isSameMinute(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisMonth (dirtyDate)](#apidoc.element.date-fns.isThisMonth)
- description and source-code
```javascript
function isThisMonth(dirtyDate) {
  return isSameMonth(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisQuarter (dirtyDate)](#apidoc.element.date-fns.isThisQuarter)
- description and source-code
```javascript
function isThisQuarter(dirtyDate) {
  return isSameQuarter(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisSecond"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisSecond (dirtyDate)](#apidoc.element.date-fns.isThisSecond)
- description and source-code
```javascript
function isThisSecond(dirtyDate) {
  return isSameSecond(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.isThisWeek)
- description and source-code
```javascript
function isThisWeek(dirtyDate, dirtyOptions) {
  return isSameWeek(new Date(), dirtyDate, dirtyOptions)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThisYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThisYear (dirtyDate)](#apidoc.element.date-fns.isThisYear)
- description and source-code
```javascript
function isThisYear(dirtyDate) {
  return isSameYear(new Date(), dirtyDate)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isThursday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isThursday (dirtyDate)](#apidoc.element.date-fns.isThursday)
- description and source-code
```javascript
function isThursday(dirtyDate) {
  return parse(dirtyDate).getDay() === 4
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isToday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isToday (dirtyDate)](#apidoc.element.date-fns.isToday)
- description and source-code
```javascript
function isToday(dirtyDate) {
  return startOfDay(dirtyDate).getTime() === startOfDay(new Date()).getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isTomorrow"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isTomorrow (dirtyDate)](#apidoc.element.date-fns.isTomorrow)
- description and source-code
```javascript
function isTomorrow(dirtyDate) {
  var tomorrow = new Date()
  tomorrow.setDate(tomorrow.getDate() + 1)
  return startOfDay(dirtyDate).getTime() === startOfDay(tomorrow).getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isTuesday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isTuesday (dirtyDate)](#apidoc.element.date-fns.isTuesday)
- description and source-code
```javascript
function isTuesday(dirtyDate) {
  return parse(dirtyDate).getDay() === 2
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isValid"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isValid (dirtyDate)](#apidoc.element.date-fns.isValid)
- description and source-code
```javascript
function isValid(dirtyDate) {
  if (isDate(dirtyDate)) {
    return !isNaN(dirtyDate)
  } else {
    throw new TypeError(toString.call(dirtyDate) + ' is not an instance of Date')
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isWednesday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isWednesday (dirtyDate)](#apidoc.element.date-fns.isWednesday)
- description and source-code
```javascript
function isWednesday(dirtyDate) {
  return parse(dirtyDate).getDay() === 3
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isWeekend"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isWeekend (dirtyDate)](#apidoc.element.date-fns.isWeekend)
- description and source-code
```javascript
function isWeekend(dirtyDate) {
  var date = parse(dirtyDate)
  var day = date.getDay()
  return day === 0 || day === 6
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isWithinRange"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isWithinRange (dirtyDate, dirtyStartDate, dirtyEndDate)](#apidoc.element.date-fns.isWithinRange)
- description and source-code
```javascript
function isWithinRange(dirtyDate, dirtyStartDate, dirtyEndDate) {
  var time = parse(dirtyDate).getTime()
  var startTime = parse(dirtyStartDate).getTime()
  var endTime = parse(dirtyEndDate).getTime()

  if (startTime > endTime) {
    throw new Error('The start of the range cannot be after the end of the range')
  }

  return time >= startTime && time <= endTime
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.isYesterday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>isYesterday (dirtyDate)](#apidoc.element.date-fns.isYesterday)
- description and source-code
```javascript
function isYesterday(dirtyDate) {
  var yesterday = new Date()
  yesterday.setDate(yesterday.getDate() - 1)
  return startOfDay(dirtyDate).getTime() === startOfDay(yesterday).getTime()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.lastDayOfISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfISOWeek (dirtyDate)](#apidoc.element.date-fns.lastDayOfISOWeek)
- description and source-code
```javascript
function lastDayOfISOWeek(dirtyDate) {
  return lastDayOfWeek(dirtyDate, {weekStartsOn: 1})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.lastDayOfISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfISOYear (dirtyDate)](#apidoc.element.date-fns.lastDayOfISOYear)
- description and source-code
```javascript
function lastDayOfISOYear(dirtyDate) {
  var year = getISOYear(dirtyDate)
  var fourthOfJanuary = new Date(0)
  fourthOfJanuary.setFullYear(year + 1, 0, 4)
  fourthOfJanuary.setHours(0, 0, 0, 0)
  var date = startOfISOWeek(fourthOfJanuary)
  date.setDate(date.getDate() - 1)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.lastDayOfMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfMonth (dirtyDate)](#apidoc.element.date-fns.lastDayOfMonth)
- description and source-code
```javascript
function lastDayOfMonth(dirtyDate) {
  var date = parse(dirtyDate)
  var month = date.getMonth()
  date.setFullYear(date.getFullYear(), month + 1, 0)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.lastDayOfQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfQuarter (dirtyDate)](#apidoc.element.date-fns.lastDayOfQuarter)
- description and source-code
```javascript
function lastDayOfQuarter(dirtyDate) {
  var date = parse(dirtyDate)
  var currentMonth = date.getMonth()
  var month = currentMonth - currentMonth % 3 + 3
  date.setMonth(month, 0)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.lastDayOfWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.lastDayOfWeek)
- description and source-code
```javascript
function lastDayOfWeek(dirtyDate, dirtyOptions) {
  var weekStartsOn = dirtyOptions ? (Number(dirtyOptions.weekStartsOn) || 0) : 0

  var date = parse(dirtyDate)
  var day = date.getDay()
  var diff = (day < weekStartsOn ? -7 : 0) + 6 - (day - weekStartsOn)

  date.setHours(0, 0, 0, 0)
  date.setDate(date.getDate() + diff)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.lastDayOfYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>lastDayOfYear (dirtyDate)](#apidoc.element.date-fns.lastDayOfYear)
- description and source-code
```javascript
function lastDayOfYear(dirtyDate) {
  var date = parse(dirtyDate)
  var year = date.getFullYear()
  date.setFullYear(year + 1, 0, 0)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.max"></a>[function <span class="apidocSignatureSpan">date-fns.</span>max ()](#apidoc.element.date-fns.max)
- description and source-code
```javascript
function max() {
  var dirtyDates = Array.prototype.slice.call(arguments)
  var dates = dirtyDates.map(function (dirtyDate) {
    return parse(dirtyDate)
  })
  var latestTimestamp = Math.max.apply(null, dates)
  return new Date(latestTimestamp)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.min"></a>[function <span class="apidocSignatureSpan">date-fns.</span>min ()](#apidoc.element.date-fns.min)
- description and source-code
```javascript
function min() {
  var dirtyDates = Array.prototype.slice.call(arguments)
  var dates = dirtyDates.map(function (dirtyDate) {
    return parse(dirtyDate)
  })
  var earliestTimestamp = Math.min.apply(null, dates)
  return new Date(earliestTimestamp)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.parse"></a>[function <span class="apidocSignatureSpan">date-fns.</span>parse (argument, dirtyOptions)](#apidoc.element.date-fns.parse)
- description and source-code
```javascript
function parse(argument, dirtyOptions) {
  if (isDate(argument)) {
    // Prevent the date to lose the milliseconds when passed to new Date() in IE10
    return new Date(argument.getTime())
  } else if (typeof argument !== 'string') {
    return new Date(argument)
  }

  var options = dirtyOptions || {}
  var additionalDigits = options.additionalDigits
  if (additionalDigits == null) {
    additionalDigits = DEFAULT_ADDITIONAL_DIGITS
  } else {
    additionalDigits = Number(additionalDigits)
  }

  var dateStrings = splitDateString(argument)

  var parseYearResult = parseYear(dateStrings.date, additionalDigits)
  var year = parseYearResult.year
  var restDateString = parseYearResult.restDateString

  var date = parseDate(restDateString, year)

  if (date) {
    var timestamp = date.getTime()
    var time = 0
    var offset

    if (dateStrings.time) {
      time = parseTime(dateStrings.time)
    }

    if (dateStrings.timezone) {
      offset = parseTimezone(dateStrings.timezone)
    } else {
      // get offset accurate to hour in timezones that change offset
      offset = new Date(timestamp + time).getTimezoneOffset()
      offset = new Date(timestamp + time + offset * MILLISECONDS_IN_MINUTE).getTimezoneOffset()
    }

    return new Date(timestamp + time + offset * MILLISECONDS_IN_MINUTE)
  } else {
    return new Date(argument)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setDate"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setDate (dirtyDate, dirtyDayOfMonth)](#apidoc.element.date-fns.setDate)
- description and source-code
```javascript
function setDate(dirtyDate, dirtyDayOfMonth) {
  var date = parse(dirtyDate)
  var dayOfMonth = Number(dirtyDayOfMonth)
  date.setDate(dayOfMonth)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setDay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setDay (dirtyDate, dirtyDay, dirtyOptions)](#apidoc.element.date-fns.setDay)
- description and source-code
```javascript
function setDay(dirtyDate, dirtyDay, dirtyOptions) {
  var weekStartsOn = dirtyOptions ? (Number(dirtyOptions.weekStartsOn) || 0) : 0
  var date = parse(dirtyDate)
  var day = Number(dirtyDay)
  var currentDay = date.getDay()

  var remainder = day % 7
  var dayIndex = (remainder + 7) % 7

  var diff = (dayIndex < weekStartsOn ? 7 : 0) + day - currentDay
  return addDays(date, diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setDayOfYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setDayOfYear (dirtyDate, dirtyDayOfYear)](#apidoc.element.date-fns.setDayOfYear)
- description and source-code
```javascript
function setDayOfYear(dirtyDate, dirtyDayOfYear) {
  var date = parse(dirtyDate)
  var dayOfYear = Number(dirtyDayOfYear)
  date.setMonth(0)
  date.setDate(dayOfYear)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setHours"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setHours (dirtyDate, dirtyHours)](#apidoc.element.date-fns.setHours)
- description and source-code
```javascript
function setHours(dirtyDate, dirtyHours) {
  var date = parse(dirtyDate)
  var hours = Number(dirtyHours)
  date.setHours(hours)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setISODay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setISODay (dirtyDate, dirtyDay)](#apidoc.element.date-fns.setISODay)
- description and source-code
```javascript
function setISODay(dirtyDate, dirtyDay) {
  var date = parse(dirtyDate)
  var day = Number(dirtyDay)
  var currentDay = getISODay(date)
  var diff = day - currentDay
  return addDays(date, diff)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setISOWeek (dirtyDate, dirtyISOWeek)](#apidoc.element.date-fns.setISOWeek)
- description and source-code
```javascript
function setISOWeek(dirtyDate, dirtyISOWeek) {
  var date = parse(dirtyDate)
  var isoWeek = Number(dirtyISOWeek)
  var diff = getISOWeek(date) - isoWeek
  date.setDate(date.getDate() - diff * 7)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setISOYear (dirtyDate, dirtyISOYear)](#apidoc.element.date-fns.setISOYear)
- description and source-code
```javascript
function setISOYear(dirtyDate, dirtyISOYear) {
  var date = parse(dirtyDate)
  var isoYear = Number(dirtyISOYear)
  var diff = differenceInCalendarDays(date, startOfISOYear(date))
  var fourthOfJanuary = new Date(0)
  fourthOfJanuary.setFullYear(isoYear, 0, 4)
  fourthOfJanuary.setHours(0, 0, 0, 0)
  date = startOfISOYear(fourthOfJanuary)
  date.setDate(date.getDate() + diff)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setMilliseconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setMilliseconds (dirtyDate, dirtyMilliseconds)](#apidoc.element.date-fns.setMilliseconds)
- description and source-code
```javascript
function setMilliseconds(dirtyDate, dirtyMilliseconds) {
  var date = parse(dirtyDate)
  var milliseconds = Number(dirtyMilliseconds)
  date.setMilliseconds(milliseconds)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setMinutes"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setMinutes (dirtyDate, dirtyMinutes)](#apidoc.element.date-fns.setMinutes)
- description and source-code
```javascript
function setMinutes(dirtyDate, dirtyMinutes) {
  var date = parse(dirtyDate)
  var minutes = Number(dirtyMinutes)
  date.setMinutes(minutes)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setMonth (dirtyDate, dirtyMonth)](#apidoc.element.date-fns.setMonth)
- description and source-code
```javascript
function setMonth(dirtyDate, dirtyMonth) {
  var date = parse(dirtyDate)
  var month = Number(dirtyMonth)
  var year = date.getFullYear()
  var day = date.getDate()

  var dateWithDesiredMonth = new Date(0)
  dateWithDesiredMonth.setFullYear(year, month, 15)
  dateWithDesiredMonth.setHours(0, 0, 0, 0)
  var daysInMonth = getDaysInMonth(dateWithDesiredMonth)
  // Set the last day of the new month
  // if the original date was the last day of the longer month
  date.setMonth(month, Math.min(day, daysInMonth))
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setQuarter (dirtyDate, dirtyQuarter)](#apidoc.element.date-fns.setQuarter)
- description and source-code
```javascript
function setQuarter(dirtyDate, dirtyQuarter) {
  var date = parse(dirtyDate)
  var quarter = Number(dirtyQuarter)
  var oldQuarter = Math.floor(date.getMonth() / 3) + 1
  var diff = quarter - oldQuarter
  return setMonth(date, date.getMonth() + diff * 3)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setSeconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setSeconds (dirtyDate, dirtySeconds)](#apidoc.element.date-fns.setSeconds)
- description and source-code
```javascript
function setSeconds(dirtyDate, dirtySeconds) {
  var date = parse(dirtyDate)
  var seconds = Number(dirtySeconds)
  date.setSeconds(seconds)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.setYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>setYear (dirtyDate, dirtyYear)](#apidoc.element.date-fns.setYear)
- description and source-code
```javascript
function setYear(dirtyDate, dirtyYear) {
  var date = parse(dirtyDate)
  var year = Number(dirtyYear)
  date.setFullYear(year)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfDay"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfDay (dirtyDate)](#apidoc.element.date-fns.startOfDay)
- description and source-code
```javascript
function startOfDay(dirtyDate) {
  var date = parse(dirtyDate)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfHour"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfHour (dirtyDate)](#apidoc.element.date-fns.startOfHour)
- description and source-code
```javascript
function startOfHour(dirtyDate) {
  var date = parse(dirtyDate)
  date.setMinutes(0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfISOWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfISOWeek (dirtyDate)](#apidoc.element.date-fns.startOfISOWeek)
- description and source-code
```javascript
function startOfISOWeek(dirtyDate) {
  return startOfWeek(dirtyDate, {weekStartsOn: 1})
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfISOYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfISOYear (dirtyDate)](#apidoc.element.date-fns.startOfISOYear)
- description and source-code
```javascript
function startOfISOYear(dirtyDate) {
  var year = getISOYear(dirtyDate)
  var fourthOfJanuary = new Date(0)
  fourthOfJanuary.setFullYear(year, 0, 4)
  fourthOfJanuary.setHours(0, 0, 0, 0)
  var date = startOfISOWeek(fourthOfJanuary)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfMinute"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfMinute (dirtyDate)](#apidoc.element.date-fns.startOfMinute)
- description and source-code
```javascript
function startOfMinute(dirtyDate) {
  var date = parse(dirtyDate)
  date.setSeconds(0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfMonth"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfMonth (dirtyDate)](#apidoc.element.date-fns.startOfMonth)
- description and source-code
```javascript
function startOfMonth(dirtyDate) {
  var date = parse(dirtyDate)
  date.setDate(1)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfQuarter"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfQuarter (dirtyDate)](#apidoc.element.date-fns.startOfQuarter)
- description and source-code
```javascript
function startOfQuarter(dirtyDate) {
  var date = parse(dirtyDate)
  var currentMonth = date.getMonth()
  var month = currentMonth - currentMonth % 3
  date.setMonth(month, 1)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfSecond"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfSecond (dirtyDate)](#apidoc.element.date-fns.startOfSecond)
- description and source-code
```javascript
function startOfSecond(dirtyDate) {
  var date = parse(dirtyDate)
  date.setMilliseconds(0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfToday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfToday ()](#apidoc.element.date-fns.startOfToday)
- description and source-code
```javascript
function startOfToday() {
  return startOfDay(new Date())
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfTomorrow"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfTomorrow ()](#apidoc.element.date-fns.startOfTomorrow)
- description and source-code
```javascript
function startOfTomorrow() {
  var now = new Date()
  var year = now.getFullYear()
  var month = now.getMonth()
  var day = now.getDate()

  var date = new Date(0)
  date.setFullYear(year, month, day + 1)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfWeek"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfWeek (dirtyDate, dirtyOptions)](#apidoc.element.date-fns.startOfWeek)
- description and source-code
```javascript
function startOfWeek(dirtyDate, dirtyOptions) {
  var weekStartsOn = dirtyOptions ? (Number(dirtyOptions.weekStartsOn) || 0) : 0

  var date = parse(dirtyDate)
  var day = date.getDay()
  var diff = (day < weekStartsOn ? 7 : 0) + day - weekStartsOn

  date.setDate(date.getDate() - diff)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfYear"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfYear (dirtyDate)](#apidoc.element.date-fns.startOfYear)
- description and source-code
```javascript
function startOfYear(dirtyDate) {
  var cleanDate = parse(dirtyDate)
  var date = new Date(0)
  date.setFullYear(cleanDate.getFullYear(), 0, 1)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.startOfYesterday"></a>[function <span class="apidocSignatureSpan">date-fns.</span>startOfYesterday ()](#apidoc.element.date-fns.startOfYesterday)
- description and source-code
```javascript
function startOfYesterday() {
  var now = new Date()
  var year = now.getFullYear()
  var month = now.getMonth()
  var day = now.getDate()

  var date = new Date(0)
  date.setFullYear(year, month, day - 1)
  date.setHours(0, 0, 0, 0)
  return date
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subDays"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subDays (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subDays)
- description and source-code
```javascript
function subDays(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addDays(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subHours"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subHours (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subHours)
- description and source-code
```javascript
function subHours(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addHours(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subISOYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subISOYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subISOYears)
- description and source-code
```javascript
function subISOYears(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addISOYears(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subMilliseconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subMilliseconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subMilliseconds)
- description and source-code
```javascript
function subMilliseconds(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMilliseconds(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subMinutes"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subMinutes (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subMinutes)
- description and source-code
```javascript
function subMinutes(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMinutes(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subMonths"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subMonths (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subMonths)
- description and source-code
```javascript
function subMonths(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addMonths(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subQuarters"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subQuarters (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subQuarters)
- description and source-code
```javascript
function subQuarters(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addQuarters(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subSeconds"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subSeconds (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subSeconds)
- description and source-code
```javascript
function subSeconds(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addSeconds(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subWeeks"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subWeeks (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subWeeks)
- description and source-code
```javascript
function subWeeks(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addWeeks(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.date-fns.subYears"></a>[function <span class="apidocSignatureSpan">date-fns.</span>subYears (dirtyDate, dirtyAmount)](#apidoc.element.date-fns.subYears)
- description and source-code
```javascript
function subYears(dirtyDate, dirtyAmount) {
  var amount = Number(dirtyAmount)
  return addYears(dirtyDate, -amount)
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
