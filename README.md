# api documentation for  [node-webkit-builder (v1.0.13)](https://github.com/mllrsohn/node-webkit-builder)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-webkit-builder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-webkit-builder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-webkit-builder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-webkit-builder)
#### node-webkit-builder

[![NPM](https://nodei.co/npm/node-webkit-builder.png?downloads=true)](https://www.npmjs.com/package/node-webkit-builder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-webkit-builder_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-webkit-builder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Steffen Müller"
    },
    "bin": {
        "nwbuild": "./bin/nwbuild"
    },
    "bugs": {
        "url": "https://github.com/mllrsohn/node-webkit-builder/issues"
    },
    "dependencies": {
        "archiver": "^0.13.0",
        "bluebird": "~1.2.2",
        "decompress-zip": "0.0.8",
        "graceful-fs-extra": "^1.0.4",
        "graceful-ncp": "^2.0.0",
        "inherits": "~2.0.1",
        "lodash": "~2.4.1",
        "optimist": "^0.6.1",
        "platform-overrides": "~1.0.1",
        "plist": "^1.0.0",
        "progress": "~1.1.7",
        "rcedit": "0.2.0",
        "request": "~2.40.0",
        "rimraf": "^2.2.8",
        "semver": "^2.3.1",
        "simple-glob": "~0.1.0",
        "tar-fs": "^0.3.2",
        "temp": "~0.7.0",
        "update-notifier": "^0.1.8",
        "winresourcer": "^0.9.0"
    },
    "deprecated": "WARNING: This module has been renamed to nw-builder. Install using nw-builder instead, node-webkit-builder will no longer be updated.",
    "description": "node-webkit-builder",
    "devDependencies": {
        "colortape": "~0.1.0",
        "nock": "^0.32.3",
        "redtape": "~1.0.0",
        "tape": "~3.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "050a6614263960cb8fd1fa7824911525f2c66b0b",
        "tarball": "https://registry.npmjs.org/node-webkit-builder/-/node-webkit-builder-1.0.13.tgz"
    },
    "gitHead": "896d8cbe7512e80f12114df152c765cc071bd279",
    "homepage": "https://github.com/mllrsohn/node-webkit-builder",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "steffen",
            "email": "steffen@mllrsohn.com"
        },
        {
            "name": "adam-lynch",
            "email": "contact@adamlynch.ie"
        },
        {
            "name": "gabepaez",
            "email": "gabe.paez@gmail.com"
        },
        {
            "name": "dylangattey",
            "email": "dylan.gattey@gmail.com"
        },
        {
            "name": "trevorah",
            "email": "a.trevorah@gmail.com"
        }
    ],
    "name": "node-webkit-builder",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/mllrsohn/node-webkit-builder.git"
    },
    "scripts": {
        "test": "colortape test/*.js"
    },
    "version": "1.0.13"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-webkit-builder](#apidoc.module.node-webkit-builder)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.</span>super_ ()](#apidoc.element.node-webkit-builder.super_)
1.  object <span class="apidocSignatureSpan">node-webkit-builder.</span>downloader
1.  object <span class="apidocSignatureSpan">node-webkit-builder.</span>utils
1.  object <span class="apidocSignatureSpan">node-webkit-builder.</span>versions

#### [module node-webkit-builder.downloader](#apidoc.module.node-webkit-builder.downloader)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>checkCache (cachepath, files)](#apidoc.element.node-webkit-builder.downloader.checkCache)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>clearProgressbar ()](#apidoc.element.node-webkit-builder.downloader.clearProgressbar)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>downloadAndUnpack (cachepath, url)](#apidoc.element.node-webkit-builder.downloader.downloadAndUnpack)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>extractTar (tarstream, destination)](#apidoc.element.node-webkit-builder.downloader.extractTar)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>extractZip (zipfile, destination)](#apidoc.element.node-webkit-builder.downloader.extractZip)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>stripRootFolder (extracted)](#apidoc.element.node-webkit-builder.downloader.stripRootFolder)

#### [module node-webkit-builder.utils](#apidoc.module.node-webkit-builder.utils)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>closerPathDepth (path1, path2)](#apidoc.element.node-webkit-builder.utils.closerPathDepth)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>copyFile (src, dest, _event)](#apidoc.element.node-webkit-builder.utils.copyFile)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>editPlist (plistInput, plistOutput, options)](#apidoc.element.node-webkit-builder.utils.editPlist)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>generateZipFile (files, _event, platformSpecificManifest)](#apidoc.element.node-webkit-builder.utils.generateZipFile)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>getFileList (fileglob)](#apidoc.element.node-webkit-builder.utils.getFileList)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>getPackageInfo (path)](#apidoc.element.node-webkit-builder.utils.getPackageInfo)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>getPlistOptions (parsedParams, custom)](#apidoc.element.node-webkit-builder.utils.getPlistOptions)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>mergeFiles (app, zipfile, chmod)](#apidoc.element.node-webkit-builder.utils.mergeFiles)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>pathDepth (absolutePath)](#apidoc.element.node-webkit-builder.utils.pathDepth)

#### [module node-webkit-builder.versions](#apidoc.module.node-webkit-builder.versions)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.versions.</span>getLatestVersion (url)](#apidoc.element.node-webkit-builder.versions.getLatestVersion)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.versions.</span>getVersionNames (v)](#apidoc.element.node-webkit-builder.versions.getVersionNames)
1.  [function <span class="apidocSignatureSpan">node-webkit-builder.versions.</span>getVersions (url)](#apidoc.element.node-webkit-builder.versions.getVersions)



# <a name="apidoc.module.node-webkit-builder"></a>[module node-webkit-builder](#apidoc.module.node-webkit-builder)

#### <a name="apidoc.element.node-webkit-builder.super_"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.</span>super_ ()](#apidoc.element.node-webkit-builder.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-webkit-builder.downloader"></a>[module node-webkit-builder.downloader](#apidoc.module.node-webkit-builder.downloader)

#### <a name="apidoc.element.node-webkit-builder.downloader.checkCache"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>checkCache (cachepath, files)](#apidoc.element.node-webkit-builder.downloader.checkCache)
- description and source-code
```javascript
checkCache = function (cachepath, files) {
    var missing;
    files.forEach(function(file) {
        if (missing) {
            return;
        }
        if (!fs.existsSync(path.join(cachepath, file))) {
            missing = true;
        }
    });

    return !missing;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.downloader.clearProgressbar"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>clearProgressbar ()](#apidoc.element.node-webkit-builder.downloader.clearProgressbar)
- description and source-code
```javascript
clearProgressbar = function () {
    bar && bar.terminate();
    bar = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.downloader.downloadAndUnpack"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>downloadAndUnpack (cachepath, url)](#apidoc.element.node-webkit-builder.downloader.downloadAndUnpack)
- description and source-code
```javascript
downloadAndUnpack = function (cachepath, url) {
    var extention = path.extname(url),
        done = Promise.defer(),
        self = this,
        rq = request(url),
        len,
        stream;

    function format(statusCode) {
        return statusCode + ': ' + require('http').STATUS_CODES[statusCode];
    }

    rq.proxy = true;
    rq.on('error', function(err) {
        bar && bar.terminate();
        done.reject(err);
    });
    rq.on('response', function (res) {
        len = parseInt(res.headers['content-length'], 10);
        if (res.statusCode !== 200) {
            done.reject({
                statusCode: res.statusCode,
                msg: 'Recieved status code ' + format(res.statusCode)
            });
        } else if (len) {
            if (!bar) {
                bar = new progress('  downloading [:bar] :percent :etas', {
                    complete: '=',
                    incomplete: '-',
                    width: 20,
                    total: len
                });
            } else {
                bar.total += len;
            }
        }
    });
    rq.on('data', function(chunk) {
        len && bar && bar.tick(chunk.length);
    });

    if (extention === '.zip') {
        stream = temp.createWriteStream();

        stream.on('close', function() {
            if(done.promise.isRejected()) return;
            self.extractZip(stream.path, cachepath).then(self.stripRootFolder).then(function(files) {
                done.resolve(files);
            });
        });

        rq.pipe(stream);
    }

    if (extention === '.gz') {
        rq.on('response', function(res) {
            if(res.statusCode !== 200) return;
            self.extractTar(res, cachepath).then(self.stripRootFolder).then(function(files) {
                done.resolve(files);
            });
        });
    }

    return done.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.downloader.extractTar"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>extractTar (tarstream, destination)](#apidoc.element.node-webkit-builder.downloader.extractTar)
- description and source-code
```javascript
extractTar = function (tarstream, destination) {
    var done = Promise.defer(),
        gunzip = zlib.createGunzip(),
        files = [];

    tarstream
        .pipe(gunzip)
        .on('error', function(err){
            done.reject(err);
        })
        .pipe(tar.extract(destination, {
            umask: (isWin ? false : 0),
            map: function(header) {
                files.push({path: path.basename(header.name)});
                return header;
            }
        }))
        .on('finish', function() {
            done.resolve({files:files, destination:destination});
        });

    return done.promise;
}
```
- example usage
```shell
...

        rq.pipe(stream);
    }

    if (extention === '.gz') {
        rq.on('response', function(res) {
            if(res.statusCode !== 200) return;
            self.extractTar(res, cachepath).then(self.stripRootFolder).then(function(files) {
                done.resolve(files);
            });
        });
    }

    return done.promise;
},
...
```

#### <a name="apidoc.element.node-webkit-builder.downloader.extractZip"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>extractZip (zipfile, destination)](#apidoc.element.node-webkit-builder.downloader.extractZip)
- description and source-code
```javascript
extractZip = function (zipfile, destination) {
    var files = [],
        done = Promise.defer();

    new DecompressZip(zipfile)
        .on('error', function(err){
            done.reject(err);
        })
        .on('extract', function(log) {
            // Setup chmodSync to fix permissions
            files.forEach(function(file) {
                fs.chmodSync(path.join(destination, file.path), file.mode);
            });

            done.resolve({files:files, destination:destination});
        })
        .extract({
            path: destination,
            filter: function(entry) {
                files.push({
                    path: entry.path,
                    mode: entry.mode.toString(8)
                });

                return true;
            }
        });

    return done.promise;
}
```
- example usage
```shell
...
});

if (extention === '.zip') {
    stream = temp.createWriteStream();

    stream.on('close', function() {
        if(done.promise.isRejected()) return;
        self.extractZip(stream.path, cachepath).then(self.stripRootFolder).then(function(files) {
            done.resolve(files);
        });
    });

    rq.pipe(stream);
}
...
```

#### <a name="apidoc.element.node-webkit-builder.downloader.stripRootFolder"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.downloader.</span>stripRootFolder (extracted)](#apidoc.element.node-webkit-builder.downloader.stripRootFolder)
- description and source-code
```javascript
stripRootFolder = function (extracted){
    var done = Promise.defer(),
        files = extracted.files,
        destination = extracted.destination,
        rootFiles = fs.readdirSync(destination),
        fromDir = path.join(destination, rootFiles.length === 1 ? rootFiles[0] : '');

    // strip out root folder if it exists
    if(rootFiles.length === 1 && fs.statSync(fromDir).isDirectory() ){
        // strip folder from files
        for (var i = 0; i < files.length; i++) {
            var file = files[i];
            file.path = path.relative(rootFiles[0], file.path);
            if(file.path === '') {
                files.splice(i, 1);
                i--;
            }
        }
        // move stripped folder to destination
        ncp(fromDir, destination, function (err) {
            if (err) done.reject();
            else rimraf(fromDir, function(){
                done.resolve(files);
            });
        });
    } else {
        done.resolve(files);
    }

    return done.promise;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-webkit-builder.utils"></a>[module node-webkit-builder.utils](#apidoc.module.node-webkit-builder.utils)

#### <a name="apidoc.element.node-webkit-builder.utils.closerPathDepth"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>closerPathDepth (path1, path2)](#apidoc.element.node-webkit-builder.utils.closerPathDepth)
- description and source-code
```javascript
closerPathDepth = function (path1, path2) {
    if (!path2) { return path1; }

    var d1 = this.pathDepth(path1),
        d2 = this.pathDepth(path2);

    return d1 < d2 ? path1 : path2;
}
```
- example usage
```shell
...

        return new Promise(function(resolve, reject) {
if(!matches.length) return reject('No files matching');

matches.forEach(function(file) {
    var internalFileName = path.normalize(file);
    if (internalFileName.match('package.json')) {
        jsonfile = self.closerPathDepth(internalFileName, jsonfile);
        package_path = path.normalize(jsonfile.split('package.json')[0] || './');
    }
    if(!fs.lstatSync(internalFileName).isDirectory()) {
        srcFiles.push(internalFileName);
    }
});
...
```

#### <a name="apidoc.element.node-webkit-builder.utils.copyFile"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>copyFile (src, dest, _event)](#apidoc.element.node-webkit-builder.utils.copyFile)
- description and source-code
```javascript
copyFile = function (src, dest, _event) {
    return new Promise(function(resolve, reject) {
        var stats = fs.lstatSync(src);
        fs.copy(src, dest, function (err) {
            if(err) return reject(err);

            var retryCount = 0;
            var existsCallback = function(exists){
                if(exists){
                    fs.chmod(dest, stats.mode, function(err){
                        // ignore error
                        if (err) {
                            _event.emit('log', 'chmod ' + stats.mode + ' on ' + dest + ' failed after copying, ignoring');
                        }

                        resolve();
                    });
                } else if (retryCount++ < 2) {
                    // This is antipattern!!!
                    // Callback should be called when the copy is finished!!!!
                    setTimeout(function(){
                        fs.exists(dest, existsCallback);
                    }, 1000);
                } else {
                    reject(new Error("Copied file (" + dest + ") doesn't exist in destination after copying"));
                }
            }

            fs.exists(dest, existsCallback);
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.editPlist"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>editPlist (plistInput, plistOutput, options)](#apidoc.element.node-webkit-builder.utils.editPlist)
- description and source-code
```javascript
editPlist = function (plistInput, plistOutput, options) {
    options = options || {};

    // Make sure all required properties are set
    [
        'CFBundleName',
        'CFBundleDisplayName',
        'CFBundleVersion',
        'CFBundleShortVersionString'
    ].forEach(function(prop) {
            if(!options.hasOwnProperty(prop)) {
                throw new Error('Missing macPlist property \'' + prop + '\'');
            }
        });

    // Bundle identifier based on package name
    if(options.CFBundleIdentifier === undefined) {
        options.CFBundleIdentifier = 'com.node-webkit-builder.' + options.CFBundleName.toLowerCase().replace(/[^a-z\-]/g,'');
    }

    // Read the input file
    return readFile(plistInput, 'utf8')
        // Parse it
        .then(plist.parse)
        // Then overwrite the properties with custom values
        .then(function(info) {
            // Keep backwards compatibility and handle aliases
            Object.keys(options).forEach(function(key) {
                var value = options[key];
                switch(key) {
                    case 'mac_bundle_id':
                        info.CFBundleIdentifier = value;
                        break;
                    case 'mac_document_types':
                        info.CFBundleDocumentTypes = value.map(function(type) {
                            return {
                                CFBundleTypeName: type.name,
                                CFBundleTypeExtensions: type.extensions,
                                CFBundleTypeRole: type.role,
                                LSIsAppleDefaultForType: type.isDefault
                            };
                        });
                        break;
                    default:
                        info[key] = value;
                }
            });

            // Remove some unwanted properties
            if(!(options.hasOwnProperty('mac_document_types') || options.hasOwnProperty('CFBundleDocumentTypes'))) {
                info.CFBundleDocumentTypes = [];
            }

            if(!options.hasOwnProperty('UTExportedTypeDeclarations'))
                info.UTExportedTypeDeclarations = [];

            // Write output file
            return writeFile(plistOutput, plist.build(info));
        });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.generateZipFile"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>generateZipFile (files, _event, platformSpecificManifest)](#apidoc.element.node-webkit-builder.utils.generateZipFile)
- description and source-code
```javascript
generateZipFile = function (files, _event, platformSpecificManifest) {
    var destStream = temp.createWriteStream(),
        archive = archiver('zip');

    return new Promise(function(resolve, reject) {

        // Resolve on close
        destStream.on('close', function () {
            resolve(destStream.path);
        });

        // Reject on Error
        archive.on('error', reject);

        // Add the files
        var filesBulk = [];
        files.forEach(function(file){
            if(file.dest === 'package.json' && platformSpecificManifest){
                archive.append(platformSpecificManifest, {name: 'package.json'});
            }
            else
            {
                filesBulk.push({
                    src: file.src,
                    data: { name: path.basename(file.dest) },
                    expand: true,
                    flatten: true,
                    dest: path.dirname(file.dest)
                });
            }
        })
        archive.bulk(filesBulk)

        // Some logs
        archive.on('entry', function (file) {
            _event.emit('log', 'Zipping ' + file.name);
        });

        // Pipe the stream
        archive.pipe(destStream);
        archive.finalize();

    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.getFileList"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>getFileList (fileglob)](#apidoc.element.node-webkit-builder.utils.getFileList)
- description and source-code
```javascript
getFileList = function (fileglob) {
    var self = this,
        jsonfile, destFiles = [],
        srcFiles = [],
        package_path,
        matches = Glob(fileglob);

    return new Promise(function(resolve, reject) {
        if(!matches.length) return reject('No files matching');

        matches.forEach(function(file) {
            var internalFileName = path.normalize(file);
            if (internalFileName.match('package.json')) {
                jsonfile = self.closerPathDepth(internalFileName, jsonfile);
                package_path = path.normalize(jsonfile.split('package.json')[0] || './');
            }
            if(!fs.lstatSync(internalFileName).isDirectory()) {
                srcFiles.push(internalFileName);
            }
        });

        if (!jsonfile) {
            return reject('Could not find a package.json in your src folder');
        }

        srcFiles.forEach(function(file) {
            destFiles.push({
                src: file,
                dest: file.replace(package_path, '')
            });
        });

        resolve({
            files: destFiles,
            json: jsonfile
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.getPackageInfo"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>getPackageInfo (path)](#apidoc.element.node-webkit-builder.utils.getPackageInfo)
- description and source-code
```javascript
getPackageInfo = function (path) {
    return new Promise(function(resolve, reject) {
        fs.readFile(path, function (err, data) {
            if (err) return reject(err);
            try {
                var appPkg = JSON.parse(data);
            } catch(e) {
                reject("Invalid package.json: " + e + "\nMake sure the file is encoded as utf-8");
                return;
            }
            if (!appPkg.name || !appPkg.version) {
                reject("Please make sure that your project's package.json includes a version and a name value");
            } else {
                resolve(appPkg);
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.getPlistOptions"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>getPlistOptions (parsedParams, custom)](#apidoc.element.node-webkit-builder.utils.getPlistOptions)
- description and source-code
```javascript
getPlistOptions = function (parsedParams, custom) {
    var obj = {};
    if(parsedParams.name) {
        obj.CFBundleName = parsedParams.name;
        obj.CFBundleDisplayName = parsedParams.name;
    }
    if(parsedParams.version) {
        obj.CFBundleVersion = parsedParams.version;
        obj.CFBundleShortVersionString = 'Version ' + parsedParams.version;
    }
    if(parsedParams.copyright) {
        obj.NSHumanReadableCopyright = parsedParams.copyright;
    }

    return _.merge(obj, custom);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.mergeFiles"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>mergeFiles (app, zipfile, chmod)](#apidoc.element.node-webkit-builder.utils.mergeFiles)
- description and source-code
```javascript
mergeFiles = function (app, zipfile, chmod) {
    // we need to pipe the app into the zipfile and chmod it
    return new Promise(function(resolve, reject) {
        var zipStream = fs.createReadStream(zipfile),
            writeStream = fs.createWriteStream(app, {flags:'a'});

        zipStream.on('error', reject);
        writeStream.on('error', reject);

        writeStream.on('finish', function () {
            if(chmod) {
                fs.chmodSync(app, chmod);
            }
            resolve();
        });

        zipStream.pipe(writeStream);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.utils.pathDepth"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.utils.</span>pathDepth (absolutePath)](#apidoc.element.node-webkit-builder.utils.pathDepth)
- description and source-code
```javascript
pathDepth = function (absolutePath) {
    return absolutePath.split(path.sep).length;
}
```
- example usage
```shell
...
            json: jsonfile
        });
    });
},
closerPathDepth: function(path1, path2) {
    if (!path2) { return path1; }

    var d1 = this.pathDepth(path1),
        d2 = this.pathDepth(path2);

    return d1 < d2 ? path1 : path2;
},
pathDepth: function(absolutePath) {
    return absolutePath.split(path.sep).length;
},
...
```



# <a name="apidoc.module.node-webkit-builder.versions"></a>[module node-webkit-builder.versions](#apidoc.module.node-webkit-builder.versions)

#### <a name="apidoc.element.node-webkit-builder.versions.getLatestVersion"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.versions.</span>getLatestVersion (url)](#apidoc.element.node-webkit-builder.versions.getLatestVersion)
- description and source-code
```javascript
getLatestVersion = function (url) {
    return getVersionList(url)
        .then(function(versions) {
            return versions[0];
        });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-webkit-builder.versions.getVersionNames"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.versions.</span>getVersionNames (v)](#apidoc.element.node-webkit-builder.versions.getVersionNames)
- description and source-code
```javascript
getVersionNames = function (v) {
    var versionNames = {
        version: v,
        platforms: {}
    };

    var templateData = {
        version: v,
        name: semver.satisfies(v, '>=0.12.0 || ~0.12.0-alpha') ? 'nwjs' : 'node-webkit'
    };

    // create a hash of platform version names based on current platforms
    _.forEach(platforms, function (platform, name) {
        versionNames.platforms[name] = _.template(platform.versionNameTemplate, templateData);
    });

    return versionNames;
}
```
- example usage
```shell
...
versions = versions.sort(function(a,b){ return semver.compare(b,a); });

// filter out invalid / alpha versions
var validationPromises = [];
versions.forEach(function(version){
    validationPromises.push(new Promise(function(resolve, reject){
        // check if windows 64-bit ZIP exists
        request.head(resolveUrl(url, module.exports.getVersionNames(version).platforms.win64), function(err, res){
            // note: this takes a version string and replaces it with an object (will be converted back later)
            resolve({
                version: version,
                valid: !err && res.statusCode === 200
            })
        });
    }));
...
```

#### <a name="apidoc.element.node-webkit-builder.versions.getVersions"></a>[function <span class="apidocSignatureSpan">node-webkit-builder.versions.</span>getVersions (url)](#apidoc.element.node-webkit-builder.versions.getVersions)
- description and source-code
```javascript
getVersions = function (url) {
    return getVersionList(url);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
