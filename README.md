# api documentation for  [http-master (v1.2.6)](https://github.com/encharm/http-master#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-http-master.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-http-master) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-http-master.svg)](https://travis-ci.org/npmdoc/node-npmdoc-http-master)
#### Easy to setup, convenient, universal, parallel, http/https proxy daemon. Setup in 1 minute, run, configure, adapt. Proxying based on excellent node-http-proxy.

[![NPM](https://nodei.co/npm/http-master.png?downloads=true)](https://www.npmjs.com/package/http-master)

[![apidoc](https://npmdoc.github.io/node-npmdoc-http-master/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-http-master_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-http-master/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-http-master/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-http-master/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Damian Kaczmarek",
        "email": "damian@codecharm.co.uk"
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
            "name": "Damian Nowak",
            "email": "damian.nowak@atlashost.eu"
        },
        {
            "name": "Sergey Zarouski",
            "email": "sergey@webuniverse.io"
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
            "name": "rush",
            "email": "rush@rushbase.net"
        }
    ],
    "name": "http-master",
    "optionalDependencies": {
        "bufferutil": "^1.2.1",
        "codeclimate-test-reporter": "~0.3.3",
        "utf-8-validate": "^1.2.1"
    },
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module http-master](#apidoc.module.http-master)
1.  [function <span class="apidocSignatureSpan">http-master.</span>CertScanner (sslDirectory, options)](#apidoc.element.http-master.CertScanner)
1.  [function <span class="apidocSignatureSpan">http-master.</span>DispatchTable (port, params)](#apidoc.element.http-master.DispatchTable)
1.  [function <span class="apidocSignatureSpan">http-master.</span>HttpMasterWorker (config)](#apidoc.element.http-master.HttpMasterWorker)
1.  [function <span class="apidocSignatureSpan">http-master.</span>di ()](#apidoc.element.http-master.di)
1.  [function <span class="apidocSignatureSpan">http-master.</span>regexpHelper (href, match)](#apidoc.element.http-master.regexpHelper)
1.  object <span class="apidocSignatureSpan">http-master.</span>DispatchTable.prototype
1.  object <span class="apidocSignatureSpan">http-master.</span>HttpMasterWorker.prototype
1.  object <span class="apidocSignatureSpan">http-master.</span>di.prototype
1.  object <span class="apidocSignatureSpan">http-master.</span>testUtils

#### [module http-master.DispatchTable](#apidoc.module.http-master.DispatchTable)
1.  [function <span class="apidocSignatureSpan">http-master.</span>DispatchTable (port, params)](#apidoc.element.http-master.DispatchTable.DispatchTable)
1.  [function <span class="apidocSignatureSpan">http-master.DispatchTable.</span>regexpQuote (str, delimiter)](#apidoc.element.http-master.DispatchTable.regexpQuote)

#### [module http-master.DispatchTable.prototype](#apidoc.module.http-master.DispatchTable.prototype)
1.  [function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>checkPathForReq (req, entry)](#apidoc.element.http-master.DispatchTable.prototype.checkPathForReq)
1.  [function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>dispatchRequest (req, res, next)](#apidoc.element.http-master.DispatchTable.prototype.dispatchRequest)
1.  [function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>getTargetForReq (req)](#apidoc.element.http-master.DispatchTable.prototype.getTargetForReq)
1.  [function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>handleRequest (req, res, next)](#apidoc.element.http-master.DispatchTable.prototype.handleRequest)

#### [module http-master.HttpMasterWorker](#apidoc.module.http-master.HttpMasterWorker)
1.  [function <span class="apidocSignatureSpan">http-master.</span>HttpMasterWorker (config)](#apidoc.element.http-master.HttpMasterWorker.HttpMasterWorker)

#### [module http-master.HttpMasterWorker.prototype](#apidoc.module.http-master.HttpMasterWorker.prototype)
1.  [function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>gcServers (gcFinished)](#apidoc.element.http-master.HttpMasterWorker.prototype.gcServers)
1.  [function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>loadConfig (config, configLoaded)](#apidoc.element.http-master.HttpMasterWorker.prototype.loadConfig)
1.  [function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>logError (msg)](#apidoc.element.http-master.HttpMasterWorker.prototype.logError)
1.  [function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>logNotice (msg)](#apidoc.element.http-master.HttpMasterWorker.prototype.logNotice)
1.  [function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>unbindAll (unbindFinished)](#apidoc.element.http-master.HttpMasterWorker.prototype.unbindAll)

#### [module http-master.di](#apidoc.module.http-master.di)
1.  [function <span class="apidocSignatureSpan">http-master.</span>di ()](#apidoc.element.http-master.di.di)

#### [module http-master.di.prototype](#apidoc.module.http-master.di.prototype)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindInstance (name, instance)](#apidoc.element.http-master.di.prototype.bindInstance)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindResolver (name, resolver)](#apidoc.element.http-master.di.prototype.bindResolver)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindTransientType (name, type)](#apidoc.element.http-master.di.prototype.bindTransientType)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindType (name, type)](#apidoc.element.http-master.di.prototype.bindType)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>clone ()](#apidoc.element.http-master.di.prototype.clone)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>makeChild ()](#apidoc.element.http-master.di.prototype.makeChild)
1.  [function <span class="apidocSignatureSpan">http-master.di.prototype.</span>resolve (obj, overrides)](#apidoc.element.http-master.di.prototype.resolve)

#### [module http-master.testUtils](#apidoc.module.http-master.testUtils)
1.  [function <span class="apidocSignatureSpan">http-master.testUtils.</span>assurePortIsListening (port, cb)](#apidoc.element.http-master.testUtils.assurePortIsListening)
1.  [function <span class="apidocSignatureSpan">http-master.testUtils.</span>assurePortNotListening (port, cb)](#apidoc.element.http-master.testUtils.assurePortNotListening)
1.  [function <span class="apidocSignatureSpan">http-master.testUtils.</span>findPort (fn)](#apidoc.element.http-master.testUtils.findPort)
1.  [function <span class="apidocSignatureSpan">http-master.testUtils.</span>findPorts (num, cb)](#apidoc.element.http-master.testUtils.findPorts)



# <a name="apidoc.module.http-master"></a>[module http-master](#apidoc.module.http-master)

#### <a name="apidoc.element.http-master.CertScanner"></a>[function <span class="apidocSignatureSpan">http-master.</span>CertScanner (sslDirectory, options)](#apidoc.element.http-master.CertScanner)
- description and source-code
```javascript
class CertScanner extends EventEmitter {
  constructor(sslDirectory, options) {
    super();

    this.options = options;

    options = options || {};

    if(!sslDirectory) {
      throw new Error('sslDirectory as first argument is mandatory');
    }

    this.sslDirectory = sslDirectory;
    if (!sslDirectory.match(/\/$/)) {
      this.sslDirectory += '/';
    }

    this.readPart = async.memoize(function(file, maxRead, cb) {
      fs.open(file, 'r', function(err, fd) {
        if(err) return cb(err);
        var buf = new Buffer(maxRead);
        fs.read(fd, buf, 0, maxRead, null, function(err, bytesRead, buffer) {
          fs.close(fd);
          if(bytesRead < maxRead)
            return cb(err, buffer.slice(0, bytesRead).toString('utf8'));
          return cb(err, buffer.toString('utf8'));
        });
      });
    });

    var beginCertToken = '-----BEGIN CERTIFICATE-----';
    var endCertToken = '-----END CERTIFICATE-----';
    this.getCaCertsFromFile = function(certPath, cb) {
      // TODO: This can possibly be replaced with some regexp.
      this.readPart(certPath, 4*65536, function(err, certFileContent) {
        if(err) return cb(err);

        var possibleCerts = certFileContent.split(beginCertToken);
        var certs = [];
        var rawCerts = [];
        possibleCerts.forEach(function(cert) {
          var endTokenIndex = cert.indexOf(endCertToken);
          if (endTokenIndex === -1) {
            return null;
          }
          var rawCert = cert.substring(0, endTokenIndex);
          var parsedCert = beginCertToken + rawCert + endCertToken + '\n';
          try {
            certs.push(x509.parseCert(parsedCert));
            rawCerts.push(parsedCert);
          } catch(err) {

          }
        });
        cb(null, certs, rawCerts);
      });
    };

    this.getCaFor = async.memoize((certPath, cb) => {
      this.readPart(certPath, 65636, (err, rawCert) => {
        if(err) return cb(err);

        var parsedCert;
        try {
          parsedCert = x509.parseCert(rawCert);
        } catch(err) {
          return cb(err);
        }
        var caResults = [];
        var caRawResults = [];
        let processDirectory = (dirName, cb) => {
          fs.readdir(dirName, (err, files) => {

            if(err) return cb(err);

            async.filter(files, (certFile, cb) => {
              var certPath = path.join(dirName, certFile);

              fs.stat(certPath, (err, statData) => {
                if(statData.isDirectory()) {
                  return processDirectory(certPath, () => {
                    cb(null, false); // is a directory
                  });
                }

                this.getCaCertsFromFile(certPath, (err, certs, rawCerts) => {
                  if(err) return cb(null, false);

                  if (this.isDomainCert(certs)) {
                    return cb(null, false);
                  }
                  var matchingCa = certs.filter((cert, i) => {
                    var res = this.caMatches(cert, parsedCert);

                    if(res) {
                      caRawResults.push(rawCerts[i]);
                    }
                    return res;
                  });
                  return cb(null, matchingCa.length);
                });
              });
            }, function(err, ca) {
              caResults = ca.map(fileName => {
                return path.join(dirName, fileName);
              }).concat(caResults);

              cb(null);
            });
          });
        }
        processDirectory(this.sslDirectory, err => {
          if(err) return cb(err);

          function noArrayIfOne(arr) {
            return (arr.length === 1) ? arr[0] : arr;
          }

          if(caResults.length) {
            cb(null, noArrayIfOne(caResults), noArrayIfOne(caRawResults));
          }
          else {
            cb(null);
          }
        });
      });
    });
  }

  scan(cb) {
    var outputConfig = {};

    var keys = {};
    var certs = {};

    let options = this.options;

    let processDirectory = (dirName, cb) => { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.DispatchTable"></a>[function <span class="apidocSignatureSpan">http-master.</span>DispatchTable (port, params)](#apidoc.element.http-master.DispatchTable)
- description and source-code
```javascript
function DispatchTable(port, params) {
  var parseEntry = params.entryParser;
  var config = params.config;

  var self = this;
  this.requestHandler = params.requestHandler;
  this.upgradeHandler = params.upgradeHandler;
  this.table = {};
  this.regexpEntries = [];
  this.failedEntries = {};
  Object.keys(config || {}).forEach(function(entryKey) {
    var entry = config[entryKey];


    // split entry 192.168.0.0/host to
    // ['192.168.0.0', '/']
    var entryKeyData = splitFirst(entryKey);
    entryKey = entryKeyData[0];
    var entryPath = entryKeyData[1];

    if(entryPath) {
      entryPath = decodeURIComponent(entryPath);
    }
    if (parseEntry) {
      var parsedEntry = parseEntry(entry);
      assert(typeof parsedEntry !== 'undefined', 'entryParser should have returned something');
      entry = parsedEntry;
    }
    entry = {
      target: entry,
      port: port
    };
    if (entryPath) {
      entry.path = entryPath;
      var pathRegexp = getRegexpIfNeeded(entryPath, '\/');
      if (pathRegexp)
        entry.pathRegexp = pathRegexp;
    }
    entryKey = postParseKey(entryKey, entry);
    port = port || 80;

    if (entry.regexp) {
      self.regexpEntries.push(entry);
    } else {
      if (self.table[entryKey]) {
        if (self.table[entryKey] instanceof Array) {
          self.table[entryKey].push(entry);
          self.table[entryKey + ':' + port].push(entry);
        } else {
          var oldEntry = self.table[entryKey];
          self.table[entryKey] = [oldEntry, entry];
          self.table[entryKey + ':' + port] = [oldEntry, entry];
        }
      } else {
        self.table[entryKey + ':' + port] = entry;
        self.table[entryKey] = entry;
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.HttpMasterWorker"></a>[function <span class="apidocSignatureSpan">http-master.</span>HttpMasterWorker (config)](#apidoc.element.http-master.HttpMasterWorker)
- description and source-code
```javascript
function HttpMasterWorker(config) {
  config = config || {};
  this.config = config;
  this.middleware = [];
  var store = {};
  this.tlsSessionStore = config.tlsSessionStore || {
    get: function(id, cb) {
      id = id.toString('base64');
      cb(null, store[id], null);
    },
    set: function(id, data, cb) {
      id = id.toString('base64');
      store[id] = data;
      // todo cleanup old ids
      if (cb)
        cb();
    }
  };
  this.tcpServers = {};
  this.servers = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.di"></a>[function <span class="apidocSignatureSpan">http-master.</span>di ()](#apidoc.element.http-master.di)
- description and source-code
```javascript
function DI() {
  this.mapping = {};
  this.parent = null;
  this.onMissing = function(name) {
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.regexpHelper"></a>[function <span class="apidocSignatureSpan">http-master.</span>regexpHelper (href, match)](#apidoc.element.http-master.regexpHelper)
- description and source-code
```javascript
regexpHelper = function (href, match) {
  var pathMatchOffset = 0;
  return processMatch(href, match);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-master.DispatchTable"></a>[module http-master.DispatchTable](#apidoc.module.http-master.DispatchTable)

#### <a name="apidoc.element.http-master.DispatchTable.DispatchTable"></a>[function <span class="apidocSignatureSpan">http-master.</span>DispatchTable (port, params)](#apidoc.element.http-master.DispatchTable.DispatchTable)
- description and source-code
```javascript
function DispatchTable(port, params) {
  var parseEntry = params.entryParser;
  var config = params.config;

  var self = this;
  this.requestHandler = params.requestHandler;
  this.upgradeHandler = params.upgradeHandler;
  this.table = {};
  this.regexpEntries = [];
  this.failedEntries = {};
  Object.keys(config || {}).forEach(function(entryKey) {
    var entry = config[entryKey];


    // split entry 192.168.0.0/host to
    // ['192.168.0.0', '/']
    var entryKeyData = splitFirst(entryKey);
    entryKey = entryKeyData[0];
    var entryPath = entryKeyData[1];

    if(entryPath) {
      entryPath = decodeURIComponent(entryPath);
    }
    if (parseEntry) {
      var parsedEntry = parseEntry(entry);
      assert(typeof parsedEntry !== 'undefined', 'entryParser should have returned something');
      entry = parsedEntry;
    }
    entry = {
      target: entry,
      port: port
    };
    if (entryPath) {
      entry.path = entryPath;
      var pathRegexp = getRegexpIfNeeded(entryPath, '\/');
      if (pathRegexp)
        entry.pathRegexp = pathRegexp;
    }
    entryKey = postParseKey(entryKey, entry);
    port = port || 80;

    if (entry.regexp) {
      self.regexpEntries.push(entry);
    } else {
      if (self.table[entryKey]) {
        if (self.table[entryKey] instanceof Array) {
          self.table[entryKey].push(entry);
          self.table[entryKey + ':' + port].push(entry);
        } else {
          var oldEntry = self.table[entryKey];
          self.table[entryKey] = [oldEntry, entry];
          self.table[entryKey + ':' + port] = [oldEntry, entry];
        }
      } else {
        self.table[entryKey + ':' + port] = entry;
        self.table[entryKey] = entry;
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.DispatchTable.regexpQuote"></a>[function <span class="apidocSignatureSpan">http-master.DispatchTable.</span>regexpQuote (str, delimiter)](#apidoc.element.http-master.DispatchTable.regexpQuote)
- description and source-code
```javascript
function regexpQuote(str, delimiter) {
  // http://kevin.vanzonneveld.net
  // +   original by: booeyOH
  // +   improved by: Ates Goral (http://magnetiq.com)
  // +   improved by: Kevin van Zonneveld (http://kevin.vanzonneveld.net)
  // +   bugfixed by: Onno Marsman
  // +   improved by: Brett Zamir (http://brett-zamir.me)
  // *     example 1: preg_quote("$40");
  // *     returns 1: '\$40'
  // *     example 2: preg_quote("*RRRING* Hello?");
  // *     returns 2: '\*RRRING\* Hello\?'
  // *     example 3: preg_quote("\\.+*?[^]$(){}=!<>|:");
  // *     returns 3: '\\\.\+\*\?\[\^\]\$\(\)\{\}\=\!\<\>\|\:'
  return (str + '').replace(new RegExp('[.\\\\+*?\\[\\^\\]$(){}=!<>|:\\' + (delimiter || '') + '-]', 'g'), '\\$&');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-master.DispatchTable.prototype"></a>[module http-master.DispatchTable.prototype](#apidoc.module.http-master.DispatchTable.prototype)

#### <a name="apidoc.element.http-master.DispatchTable.prototype.checkPathForReq"></a>[function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>checkPathForReq (req, entry)](#apidoc.element.http-master.DispatchTable.prototype.checkPathForReq)
- description and source-code
```javascript
checkPathForReq = function (req, entry) {
  if(!entry.path)
    return true;
  var m;

  var parsedUrl = req.parsedUrl;
  var pathname = parsedUrl.pathname || '';

  try {
    pathname = decodeURIComponent(pathname);
  } catch(err) {}

  if(entry.pathRegexp) {
    m = pathname.match(entry.pathRegexp);
    if (m) {
      if(!req.match)
        req.match = [];
      for(var i = 1;i < m.length;++i) {
        req.match.push(m[i]);
      }
      return true;
    }
  }
  else if(pathname == entry.path) {
    return true;
  }
  return false;
}
```
- example usage
```shell
...

// look for specific host match first
// and generic path-only match then
[host, ''].some(function(host) {
  var entry = self.table[host];
  if (entry) {
    if (entry.target) {
      if(self.checkPathForReq(req, entry)) {
        target = entry.target
        return true;
      }
    }
    else { // multiple entries, check pathnames
      var targetEntries = entry;
      for (i = 0; i < targetEntries.length; ++i) {
...
```

#### <a name="apidoc.element.http-master.DispatchTable.prototype.dispatchRequest"></a>[function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>dispatchRequest (req, res, next)](#apidoc.element.http-master.DispatchTable.prototype.dispatchRequest)
- description and source-code
```javascript
dispatchRequest = function (req, res, next) {
  var target = this.getTargetForReq(req);
  if(target && this.requestHandler) {
    return this.requestHandler(req, res, next, target);
  }
  next();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.DispatchTable.prototype.getTargetForReq"></a>[function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>getTargetForReq (req)](#apidoc.element.http-master.DispatchTable.prototype.getTargetForReq)
- description and source-code
```javascript
getTargetForReq = function (req) {
  var i, m;
  var host = req.unicodeHost || req.headers.host || ''; // host can be undefined

  var self = this;
  var target;

  // look for specific host match first
  // and generic path-only match then
  [host, ''].some(function(host) {
    var entry = self.table[host];
    if (entry) {
      if (entry.target) {
        if(self.checkPathForReq(req, entry)) {
          target = entry.target
          return true;
        }
      }
      else { // multiple entries, check pathnames
        var targetEntries = entry;
        for (i = 0; i < targetEntries.length; ++i) {
          if(self.checkPathForReq(req, targetEntries[i])) {
            target = targetEntries[i].target;
            return true;
          }
        }
      }
    }
  });
  if(target) {
    return target;
  }
  // if host-only matches failed, look for path matches
  if (this.regexpEntries.length) {
    var regexpEntries = this.regexpEntries;
    for (i = 0; i < regexpEntries.length; ++i) {
      var entry = regexpEntries[i];
      if(!entry.regexp) {
        // TODO: research this
        continue;
      }
      m = host.match(entry.regexp);
      if (m) {
        if(!req.match)
          req.match = [];
        for(var i = 1;i < m.length;++i)
          req.match.push(m[i]);
        if(this.checkPathForReq(req, entry)) {
          return entry.target;
        }
      }
    }
  }
}
```
- example usage
```shell
...
        }
      }
    }
  }
};

DispatchTable.prototype.dispatchRequest = function(req, res, next) {
  var target = this.getTargetForReq(req);
  if(target && this.requestHandler) {
    return this.requestHandler(req, res, next, target);
  }
  next();
};

DispatchTable.prototype.handleRequest = DispatchTable.prototype.dispatchRequest;
...
```

#### <a name="apidoc.element.http-master.DispatchTable.prototype.handleRequest"></a>[function <span class="apidocSignatureSpan">http-master.DispatchTable.prototype.</span>handleRequest (req, res, next)](#apidoc.element.http-master.DispatchTable.prototype.handleRequest)
- description and source-code
```javascript
handleRequest = function (req, res, next) {
  var target = this.getTargetForReq(req);
  if(target && this.requestHandler) {
    return this.requestHandler(req, res, next, target);
  }
  next();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-master.HttpMasterWorker"></a>[module http-master.HttpMasterWorker](#apidoc.module.http-master.HttpMasterWorker)

#### <a name="apidoc.element.http-master.HttpMasterWorker.HttpMasterWorker"></a>[function <span class="apidocSignatureSpan">http-master.</span>HttpMasterWorker (config)](#apidoc.element.http-master.HttpMasterWorker.HttpMasterWorker)
- description and source-code
```javascript
function HttpMasterWorker(config) {
  config = config || {};
  this.config = config;
  this.middleware = [];
  var store = {};
  this.tlsSessionStore = config.tlsSessionStore || {
    get: function(id, cb) {
      id = id.toString('base64');
      cb(null, store[id], null);
    },
    set: function(id, data, cb) {
      id = id.toString('base64');
      store[id] = data;
      // todo cleanup old ids
      if (cb)
        cb();
    }
  };
  this.tcpServers = {};
  this.servers = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-master.HttpMasterWorker.prototype"></a>[module http-master.HttpMasterWorker.prototype](#apidoc.module.http-master.HttpMasterWorker.prototype)

#### <a name="apidoc.element.http-master.HttpMasterWorker.prototype.gcServers"></a>[function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>gcServers (gcFinished)](#apidoc.element.http-master.HttpMasterWorker.prototype.gcServers)
- description and source-code
```javascript
gcServers = function (gcFinished) {
  var self = this;
  var toClose = [];

  Object.keys(this.tcpServers).forEach(function(key) {
    var server = self.tcpServers[key];
    if (require('events').EventEmitter.listenerCount(server, 'connection') === 0) {
      toClose.push(server);
      delete self.tcpServers[key];
      if (self.cachedServers[key]) {
        self.cachedServers[key].server.removeAllListeners();
        delete self.cachedServers[key];
      }
    }
  });
  async.each(toClose, function(server, cb) {
    server.close();
    cb();
  }, gcFinished);
}
```
- example usage
```shell
...
      di.resolve(require(path.join(__dirname, '..', 'modules', moduleName)));
    } catch (err) {
      console.error("Error loading module:", moduleName, err);
    }
  });

  handleConfig.call(this, config, function(err) {
    self.gcServers(function() {
      if (configLoaded)
        configLoaded(err);
    });
  });
};

HttpMasterWorker.prototype.gcServers = function(gcFinished) {
...
```

#### <a name="apidoc.element.http-master.HttpMasterWorker.prototype.loadConfig"></a>[function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>loadConfig (config, configLoaded)](#apidoc.element.http-master.HttpMasterWorker.prototype.loadConfig)
- description and source-code
```javascript
loadConfig = function (config, configLoaded) {
  var self = this;

  var events = new EventEmitter();

  this.config = config;

  function messageHandler(msg) {
    events.emit('msg:' + msg.type, msg.data, msg.workerId);
  }
  this.handleMessage = messageHandler;

  this.unbindAll(function() {});
  if (this.di) {
    this.emit('reload');
  }
  var di = this.di = new DI();

  di.onMissing = function(name) {
    var m;
    if ((m = name.match(/(.+)Service$/))) {
      name = m[1];
      try {
        this.bindType(name + 'Service', require(path.join(__dirname, '..', 'modules/services/', name)));
      } catch (err) {
        console.log(err && err.message);
        return;
      }
      self.emit('loadService', name);
      return this.resolve(name + 'Service');
    }
  };

  di.bindInstance('di', di);
  di.bindInstance('worker', this);

  this.once('reload', function() {
    process.removeListener('msg', messageHandler);
    events.emit('reload');
    events.removeAllListeners();
  });

  di.bindInstance('events', events);
  di.bindResolver('config', function() {
    return self.config;
  });
  di.bindInstance('master', null);
  Object.keys(config.modules || {}).forEach(function(moduleName) {
    if (!config.modules[moduleName])
      return;
    var di = self.di.makeChild();
    di.bindInstance('di', di);
    di.bindInstance('moduleConfig', config.modules[moduleName]);
    try {
      di.resolve(require(path.join(__dirname, '..', 'modules', moduleName)));
    } catch (err) {
      console.error("Error loading module:", moduleName, err);
    }
  });

  handleConfig.call(this, config, function(err) {
    self.gcServers(function() {
      if (configLoaded)
        configLoaded(err);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.HttpMasterWorker.prototype.logError"></a>[function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>logError (msg)](#apidoc.element.http-master.HttpMasterWorker.prototype.logError)
- description and source-code
```javascript
logError = function (msg) {
  this.emit('logError', msg);
}
```
- example usage
```shell
...
var listenPortNumber = parseInt(m[3]);

var portConfig = config.ports[portEntry];

handlePortEntryConfig.call(self, listenHost, listenPortNumber, portConfig, function(err, server) {
  var entryString = (listenHost ? listenHost + ':' + listenPortNumber : 'port ' + listenPortNumber);
  if (err) {
    self.logError('Error while starting entry ' + entryString + ' : ' + err.toString());
    if (err.stack)
      self.logError(err.stack);
    errors[portEntry] = err;
  }
  if (server) {
    self.logNotice('Listening on port: ' + entryString);
  } else
...
```

#### <a name="apidoc.element.http-master.HttpMasterWorker.prototype.logNotice"></a>[function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>logNotice (msg)](#apidoc.element.http-master.HttpMasterWorker.prototype.logNotice)
- description and source-code
```javascript
logNotice = function (msg) {
  this.emit('logNotice', msg);
}
```
- example usage
```shell
...
    }
    if (!portEntrySslConfig.ciphers) {
      portEntrySslConfig.ciphers = 'EECDH+ECDSA+AESGCM:EECDH+aRSA+AESGCM:EECDH+ECDSA+SHA384:EECDH+ECDSA+SHA256:EECDH+aRSA+SHA384
:EECDH+aRSA+SHA256:EECDH+aRSA+AES+SHA:EECDH+aRSA+RC4:EECDH:EDH+aRSA:RC4:!aNULL:!eNULL:!LOW:!3DES:!MD5:!EXP:!PSK:!SRP:!DSS::+RC4:
RC4';
      if (portEntrySslConfig.disableWeakCiphers) {
        portEntrySslConfig.ciphers += ':!RC4';
      }
    } else if (portEntrySslConfig.disableWeakCiphers) {
      this.logNotice('disableWeakCiphers is incompatible with pre-set cipher list');
    }
  } else if (portEntrySslConfig.disableWeakCiphers) {
    this.logNotice('disableWeakCiphers is unsupported for node 0.10');
  }
}
...
```

#### <a name="apidoc.element.http-master.HttpMasterWorker.prototype.unbindAll"></a>[function <span class="apidocSignatureSpan">http-master.HttpMasterWorker.prototype.</span>unbindAll (unbindFinished)](#apidoc.element.http-master.HttpMasterWorker.prototype.unbindAll)
- description and source-code
```javascript
unbindAll = function (unbindFinished) {
  unbindAll.call(this, unbindFinished);
}
```
- example usage
```shell
...
this.config = config;

function messageHandler(msg) {
  events.emit('msg:' + msg.type, msg.data, msg.workerId);
}
this.handleMessage = messageHandler;

this.unbindAll(function() {});
if (this.di) {
  this.emit('reload');
}
var di = this.di = new DI();

di.onMissing = function(name) {
  var m;
...
```



# <a name="apidoc.module.http-master.di"></a>[module http-master.di](#apidoc.module.http-master.di)

#### <a name="apidoc.element.http-master.di.di"></a>[function <span class="apidocSignatureSpan">http-master.</span>di ()](#apidoc.element.http-master.di.di)
- description and source-code
```javascript
function DI() {
  this.mapping = {};
  this.parent = null;
  this.onMissing = function(name) {
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.http-master.di.prototype"></a>[module http-master.di.prototype](#apidoc.module.http-master.di.prototype)

#### <a name="apidoc.element.http-master.di.prototype.bindInstance"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindInstance (name, instance)](#apidoc.element.http-master.di.prototype.bindInstance)
- description and source-code
```javascript
bindInstance = function (name, instance) {
  if(this.mapping[name]) {
    throw new Error('\'' + name + '\' already bound');
  }
  this.mapping[name] = {
    resolve: function() {
      return instance;
    }
  };
}
```
- example usage
```shell
...



function createHandlers(portNumber, portConfig) {
  var self = this;

  var di = this.di.makeChild();
  di.bindInstance('di', di);

  di.bindInstance('portConfig', portConfig);
  di.bindInstance('portNumber', portNumber);

  di.onMissing = function(name) {

var m;
...
```

#### <a name="apidoc.element.http-master.di.prototype.bindResolver"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindResolver (name, resolver)](#apidoc.element.http-master.di.prototype.bindResolver)
- description and source-code
```javascript
bindResolver = function (name, resolver) {
  if(this.mapping[name]) {
    throw new Error('\'' + name + '\' already bound');
  }
  this.mapping[name] = {
    resolve: resolver
  };
}
```
- example usage
```shell
...
this.once('reload', function() {
  process.removeListener('msg', messageHandler);
  events.emit('reload');
  events.removeAllListeners();
});

di.bindInstance('events', events);
di.bindResolver('config', function() {
  return self.config;
});
di.bindInstance('master', null);
Object.keys(config.modules || {}).forEach(function(moduleName) {
  if (!config.modules[moduleName])
    return;
  var di = self.di.makeChild();
...
```

#### <a name="apidoc.element.http-master.di.prototype.bindTransientType"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindTransientType (name, type)](#apidoc.element.http-master.di.prototype.bindTransientType)
- description and source-code
```javascript
bindTransientType = function (name, type) {
  return bindTypeGeneric.call(this, false, name, type);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.di.prototype.bindType"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>bindType (name, type)](#apidoc.element.http-master.di.prototype.bindType)
- description and source-code
```javascript
bindType = function (name, type) {
  return bindTypeGeneric.call(this, true, name, type);
}
```
- example usage
```shell
...

di.onMissing = function(name) {

  var m;
  if ((m = name.match(/(.+)Middleware$/))) {
    name = m[1];
    try {
      di.bindType(name + 'Middleware', require('../' + path.join('modules/middleware/', name)));
    } catch (err) {
      console.log(err && err.message);
      return;
    }
    return di.resolve(name + 'Middleware');
  }
};
...
```

#### <a name="apidoc.element.http-master.di.prototype.clone"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>clone ()](#apidoc.element.http-master.di.prototype.clone)
- description and source-code
```javascript
clone = function () {
  var cloned = new DI();
  cloned.mapping = extend({}, this.mapping);
  cloned.parent = this.parent;
  cloned.onMissing = this.onMissing;
  return cloned;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.di.prototype.makeChild"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>makeChild ()](#apidoc.element.http-master.di.prototype.makeChild)
- description and source-code
```javascript
makeChild = function () {
  var child = construct(DI, Array.prototype.slice.apply(arguments));
  child.parent = this;
  return child;
}
```
- example usage
```shell
...
}



function createHandlers(portNumber, portConfig) {
var self = this;

var di = this.di.makeChild();
di.bindInstance('di', di);

di.bindInstance('portConfig', portConfig);
di.bindInstance('portNumber', portNumber);

di.onMissing = function(name) {
...
```

#### <a name="apidoc.element.http-master.di.prototype.resolve"></a>[function <span class="apidocSignatureSpan">http-master.di.prototype.</span>resolve (obj, overrides)](#apidoc.element.http-master.di.prototype.resolve)
- description and source-code
```javascript
resolve = function (obj, overrides) {
  var dependencyMap = extend({}, this.mapping, overrides);
  var args;
  var resolved;

  if(typeof obj === 'function') {
    args = functionParameters(obj);
    resolved = construct(obj, args.map(this.resolve.bind(this)));
  } else if(typeof obj === 'string') {
    if(dependencyMap[obj]) {
      if(dependencyMap[obj].resolve) {
        resolved = dependencyMap[obj].resolve(overrides);
      } else {
        resolved = dependencyMap[obj];
      }
    }
  } else {
    throw new Error('Unknown type to resolve');
  }

  if(typeof resolved ==='undefined' && this.onMissing) {
    resolved = this.onMissing(obj);
  }

  if(typeof resolved === 'undefined' && this.parent) { // search in parent if not found
    resolved = this.parent.resolve(obj, overrides);
  }

  if(typeof resolved === 'undefined' && !dependencyMap[obj]) {
    throw new Error('No recipe to resolve \'' + obj + '\'');
  }

  return resolved;
}
```
- example usage
```shell
...
    name = m[1];
    try {
      di.bindType(name + 'Middleware', require('../' + path.join('modules/middleware/', name)));
    } catch (err) {
      console.log(err && err.message);
      return;
    }
    return di.resolve(name + 'Middleware');
  }
};

var router = di.resolve('routerMiddleware');

// allow also for specifying 80: 'http://code2flow.com:8080'
if (typeof portConfig !== 'object' || portConfig instanceof Array) {
...
```



# <a name="apidoc.module.http-master.testUtils"></a>[module http-master.testUtils](#apidoc.module.http-master.testUtils)

#### <a name="apidoc.element.http-master.testUtils.assurePortIsListening"></a>[function <span class="apidocSignatureSpan">http-master.testUtils.</span>assurePortIsListening (port, cb)](#apidoc.element.http-master.testUtils.assurePortIsListening)
- description and source-code
```javascript
assurePortIsListening = function (port, cb) {
  var client = net.connect({
      port: port
    },
    function() {
      cb();
    });
  client.once('error', function(err) {
    throw new Error('Port ' + port + ' should have been listening');
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.testUtils.assurePortNotListening"></a>[function <span class="apidocSignatureSpan">http-master.testUtils.</span>assurePortNotListening (port, cb)](#apidoc.element.http-master.testUtils.assurePortNotListening)
- description and source-code
```javascript
assurePortNotListening = function (port, cb) {
  var client = net.connect({
      port: port
    },
    function() {
      throw new Error('Port ' + port + ' should have been not listening');
    });
  client.once('error', function(err) {
    cb();
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.http-master.testUtils.findPort"></a>[function <span class="apidocSignatureSpan">http-master.testUtils.</span>findPort (fn)](#apidoc.element.http-master.testUtils.findPort)
- description and source-code
```javascript
findPort = function (fn) {
  var net = require('net')
  var tester = net.createServer();
  var port;
  tester.once('error', function (err) {
    if (err.code !== 'EADDRINUSE') return fn(err)
    exports.findPort(fn);
  })
  .once('listening', function() {
    port = tester.address().port;
    tester.once('close', function() {
      fn(null, port);
    })
    tester.close();
  })
  .listen(0);
}
```
- example usage
```shell
...

exports.findPort = function(fn) {
var net = require('net')
var tester = net.createServer();
var port;
tester.once('error', function (err) {
  if (err.code !== 'EADDRINUSE') return fn(err)
  exports.findPort(fn);
})
.once('listening', function() {
  port = tester.address().port;
  tester.once('close', function() {
    fn(null, port);
  })
  tester.close();
...
```

#### <a name="apidoc.element.http-master.testUtils.findPorts"></a>[function <span class="apidocSignatureSpan">http-master.testUtils.</span>findPorts (num, cb)](#apidoc.element.http-master.testUtils.findPorts)
- description and source-code
```javascript
findPorts = function (num, cb) {
  async.times(num, function(n, cb) {
    exports.findPort(cb);
  }, function(err, port) {
    cb(err, port);
  }, cb);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
