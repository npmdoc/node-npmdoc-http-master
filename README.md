# npmdoc-http-master

#### api documentation for  [http-master (v1.2.6)](https://github.com/encharm/http-master#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-http-master.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-http-master) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-http-master.svg)](https://travis-ci.org/npmdoc/node-npmdoc-http-master)

#### Easy to setup, convenient, universal, parallel, http/https proxy daemon. Setup in 1 minute, run, configure, adapt. Proxying based on excellent node-http-proxy.

[![NPM](https://nodei.co/npm/http-master.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/http-master)

- [https://npmdoc.github.io/node-npmdoc-http-master/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-http-master/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-http-master/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-http-master/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-http-master/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-http-master/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Damian Kaczmarek"
    },
    "bin": {
        "http-master": "./bin/http-master",
        "cert-scan": "./bin/cert-scan"
    },
    "bugs": {
        "url": "https://github.com/encharm/http-master/issues"
    },
    "contributors": [
        {
            "name": "Damian Nowak"
        },
        {
            "name": "Sergey Zarouski"
        }
    ],
    "dependencies": {
        "async": "^2.1.4",
        "bluebird": "^3.4.3",
        "bufferutil": "^1.2.1",
        "bugsnag": "1.8.0",
        "codeclimate-test-reporter": "~0.3.3",
        "compression": "^1.6.2",
        "connect-gzip-static": "^1.0.0",
        "eventemitter3": "^1.2.0",
        "extend": "3.0.0",
        "greenlock": "^2.1.11",
        "http-auth": "~2.2.9",
        "http-proxy": "^1.16.2",
        "js-yaml": "3.6.1",
        "jsonfn": "0.31.0",
        "jsonlint-lines": "1.7.1",
        "le-challenge-standalone": "^2.0.0",
        "le-sni-auto": "^2.0.1",
        "memoizee": "^0.4.1",
        "moment": "^2.17.1",
        "morgan": "1.7.0",
        "node-watch": "^0.4.0",
        "ocsp": "^1.1.0",
        "parseurl": "^1.3.1",
        "send": "^0.14.2",
        "spdy": "^3.4.0",
        "uid-number": "0.0.6",
        "utf-8-validate": "^1.2.1",
        "uuid": "^2.0.2",
        "ws": "^1.1.1",
        "x509.js": "1.0.0",
        "xregexp": "^3.1.1",
        "yargs": "^6.6.0"
    },
    "description": "Easy to setup, convenient, universal, parallel, http/https proxy daemon. Setup in 1 minute, run, configure, adapt. Proxying based on excellent node-http-proxy.",
    "devDependencies": {
        "chai": "^3.5.0",
        "fs.extra": "1.3.2",
        "istanbul": "^0.4.5",
        "mocha": "^3.0.2",
        "request": "^2.79.0",
        "request-promise": "^4.1.1",
        "should": "^11.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "4ea006338a5ac0e80b956977afa2f3fec145194c",
        "tarball": "https://registry.npmjs.org/http-master/-/http-master-1.2.6.tgz"
    },
    "gitHead": "2851248a600950df0153d0812de2e1d509d58bed",
    "homepage": "https://github.com/encharm/http-master#readme",
    "keywords": [
        "http",
        "https",
        "proxy"
    ],
    "license": "MIT",
    "main": "src/HttpMaster.js",
    "maintainers": [
        {
            "name": "rush"
        }
    ],
    "name": "http-master",
    "optionalDependencies": {
        "bufferutil": "^1.2.1",
        "codeclimate-test-reporter": "~0.3.3",
        "utf-8-validate": "^1.2.1"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/encharm/http-master.git"
    },
    "scripts": {
        "test": "istanbul cover node_modules/mocha/bin/_mocha -- -R spec tests/"
    },
    "version": "1.2.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
