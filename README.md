# npmdoc-weather-js

#### api documentation for  [weather-js (v2.0.0)](http://github.com/devfacet/weather)  [![npm package](https://img.shields.io/npm/v/npmdoc-weather-js.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-weather-js) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-weather-js.svg)](https://travis-ci.org/npmdoc/node-npmdoc-weather-js)

#### A module for obtaining weather information

[![NPM](https://nodei.co/npm/weather-js.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/weather-js)

- [https://npmdoc.github.io/node-npmdoc-weather-js/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-weather-js/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-weather-js/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-weather-js/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-weather-js/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-weather-js/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "weather-js",
    "version": "2.0.0",
    "description": "A module for obtaining weather information",
    "main": "index.js",
    "scripts": {
        "lint": "jshint --reporter node_modules/jshint-stylish *.js test/*.js",
        "lint:build": "jshint --reporter checkstyle *.js test/*.js > reports/jshint-checkstyle.xml",
        "depcheck": "dependency-check . *.js",
        "depcheck:unused": "dependency-check ./package.json --unused --no-dev *.js",
        "test:unit": "mkdir -p reports/ && NODE_ENV=test multi='spec=- xunit=reports/mocha-xunit.xml' istanbul cover _mocha -- --timeout 10000 -R mocha-multi && istanbul check-coverage",
        "test:coveralls": "cat reports/coverage/lcov.info | node_modules/coveralls/bin/coveralls.js",
        "test": "npm run lint && npm run test:unit"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/devfacet/weather.git"
    },
    "keywords": [
        "weather",
        "forecast"
    ],
    "author": "devfacet",
    "license": "MIT",
    "homepage": "http://github.com/devfacet/weather",
    "dependencies": {
        "request": "2.x.x",
        "xml2js": "0.4.x"
    },
    "devDependencies": {
        "chai": "3.5.x",
        "jshint": "2.9.x",
        "jshint-stylish": "2.2.x",
        "mocha": "3.2.x",
        "mocha-multi": "0.10.x",
        "dependency-check": "2.8.x",
        "istanbul": "0.4.x",
        "coveralls": "^2.11.16"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
