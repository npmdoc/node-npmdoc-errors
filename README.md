# api documentation for  [errors (v0.3.0)](https://github.com/bodenr/errors)  [![npm package](https://img.shields.io/npm/v/npmdoc-errors.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-errors) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-errors.svg)](https://travis-ci.org/npmdoc/node-npmdoc-errors)
#### A comprehensive, robust, yet lightweight set of error utilities for node.js enabling you to do errors more effectively.

[![NPM](https://nodei.co/npm/errors.png?downloads=true)](https://www.npmjs.com/package/errors)

[![apidoc](https://npmdoc.github.io/node-npmdoc-errors/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-errors_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-errors/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-errors/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-errors/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Boden Russell",
        "email": "bodenru@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/bodenr/errors/issues"
    },
    "dependencies": {},
    "description": "A comprehensive, robust, yet lightweight set of error utilities for node.js enabling you to do errors more effectively.",
    "devDependencies": {
        "dox-foundation": "*",
        "express": "< 4.0.0",
        "markdox": "*",
        "mocha": "*",
        "should": "< 2.0.0",
        "supertest": "*"
    },
    "directories": {
        "doc": "./doc"
    },
    "dist": {
        "shasum": "572ed0fad82ab26ba04e797828f7103dd820732f",
        "tarball": "https://registry.npmjs.org/errors/-/errors-0.3.0.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "af48c56267f4e27facb78f0c773498255f1f1966",
    "homepage": "https://github.com/bodenr/errors",
    "keywords": [
        "error",
        "exceptions",
        "express",
        "connect",
        "utilities"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "boden",
            "email": "bodensemail@gmail.com"
        }
    ],
    "name": "errors",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/bodenr/errors.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "0.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module errors](#apidoc.module.errors)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http400Error (msg, expl, fix)](#apidoc.element.errors.Http400Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http401Error (msg, expl, fix)](#apidoc.element.errors.Http401Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http402Error (msg, expl, fix)](#apidoc.element.errors.Http402Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http403Error (msg, expl, fix)](#apidoc.element.errors.Http403Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http404Error (msg, expl, fix)](#apidoc.element.errors.Http404Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http405Error (msg, expl, fix)](#apidoc.element.errors.Http405Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http406Error (msg, expl, fix)](#apidoc.element.errors.Http406Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http407Error (msg, expl, fix)](#apidoc.element.errors.Http407Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http408Error (msg, expl, fix)](#apidoc.element.errors.Http408Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http409Error (msg, expl, fix)](#apidoc.element.errors.Http409Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http410Error (msg, expl, fix)](#apidoc.element.errors.Http410Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http411Error (msg, expl, fix)](#apidoc.element.errors.Http411Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http412Error (msg, expl, fix)](#apidoc.element.errors.Http412Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http413Error (msg, expl, fix)](#apidoc.element.errors.Http413Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http414Error (msg, expl, fix)](#apidoc.element.errors.Http414Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http415Error (msg, expl, fix)](#apidoc.element.errors.Http415Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http416Error (msg, expl, fix)](#apidoc.element.errors.Http416Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http417Error (msg, expl, fix)](#apidoc.element.errors.Http417Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http418Error (msg, expl, fix)](#apidoc.element.errors.Http418Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http421Error (msg, expl, fix)](#apidoc.element.errors.Http421Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http422Error (msg, expl, fix)](#apidoc.element.errors.Http422Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http423Error (msg, expl, fix)](#apidoc.element.errors.Http423Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http424Error (msg, expl, fix)](#apidoc.element.errors.Http424Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http425Error (msg, expl, fix)](#apidoc.element.errors.Http425Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http426Error (msg, expl, fix)](#apidoc.element.errors.Http426Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http428Error (msg, expl, fix)](#apidoc.element.errors.Http428Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http429Error (msg, expl, fix)](#apidoc.element.errors.Http429Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http431Error (msg, expl, fix)](#apidoc.element.errors.Http431Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http451Error (msg, expl, fix)](#apidoc.element.errors.Http451Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http500Error (msg, expl, fix)](#apidoc.element.errors.Http500Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http501Error (msg, expl, fix)](#apidoc.element.errors.Http501Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http502Error (msg, expl, fix)](#apidoc.element.errors.Http502Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http503Error (msg, expl, fix)](#apidoc.element.errors.Http503Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http504Error (msg, expl, fix)](#apidoc.element.errors.Http504Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http505Error (msg, expl, fix)](#apidoc.element.errors.Http505Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http506Error (msg, expl, fix)](#apidoc.element.errors.Http506Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http507Error (msg, expl, fix)](#apidoc.element.errors.Http507Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http508Error (msg, expl, fix)](#apidoc.element.errors.Http508Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http509Error (msg, expl, fix)](#apidoc.element.errors.Http509Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http510Error (msg, expl, fix)](#apidoc.element.errors.Http510Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http511Error (msg, expl, fix)](#apidoc.element.errors.Http511Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>HttpError (msg, expl, fix)](#apidoc.element.errors.HttpError)
1.  [function <span class="apidocSignatureSpan">errors.</span>HttpError.super_ ()](#apidoc.element.errors.HttpError.super_)
1.  [function <span class="apidocSignatureSpan">errors.</span>create (options)](#apidoc.element.errors.create)
1.  [function <span class="apidocSignatureSpan">errors.</span>errorToJSON (err, attrMap)](#apidoc.element.errors.errorToJSON)
1.  [function <span class="apidocSignatureSpan">errors.</span>find (err)](#apidoc.element.errors.find)
1.  [function <span class="apidocSignatureSpan">errors.</span>isError (err)](#apidoc.element.errors.isError)
1.  [function <span class="apidocSignatureSpan">errors.</span>mapError (err)](#apidoc.element.errors.mapError)
1.  [function <span class="apidocSignatureSpan">errors.</span>mapper (errName, fn)](#apidoc.element.errors.mapper)
1.  [function <span class="apidocSignatureSpan">errors.</span>stacks (useStacks)](#apidoc.element.errors.stacks)
1.  [function <span class="apidocSignatureSpan">errors.</span>title (title)](#apidoc.element.errors.title)
1.  object <span class="apidocSignatureSpan">errors.</span>Http400Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http401Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http402Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http403Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http404Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http405Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http406Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http407Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http408Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http409Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http410Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http411Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http412Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http413Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http414Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http415Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http416Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http417Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http418Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http421Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http422Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http423Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http424Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http425Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http426Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http428Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http429Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http431Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http451Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http500Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http501Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http502Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http503Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http504Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http505Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http506Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http507Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http508Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http509Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http510Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>Http511Error.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>HttpError.prototype
1.  object <span class="apidocSignatureSpan">errors.</span>JS_ERRORS

#### [module errors.Http400Error](#apidoc.module.errors.Http400Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http400Error (msg, expl, fix)](#apidoc.element.errors.Http400Error.Http400Error)
1.  [function <span class="apidocSignatureSpan">errors.Http400Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http400Error.super_)

#### [module errors.Http400Error.prototype](#apidoc.module.errors.Http400Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http400Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http400Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http400Error.prototype.</span>toString ()](#apidoc.element.errors.Http400Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http400Error.prototype.</span>name

#### [module errors.Http401Error](#apidoc.module.errors.Http401Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http401Error (msg, expl, fix)](#apidoc.element.errors.Http401Error.Http401Error)
1.  [function <span class="apidocSignatureSpan">errors.Http401Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http401Error.super_)

#### [module errors.Http401Error.prototype](#apidoc.module.errors.Http401Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http401Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http401Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http401Error.prototype.</span>toString ()](#apidoc.element.errors.Http401Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http401Error.prototype.</span>name

#### [module errors.Http402Error](#apidoc.module.errors.Http402Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http402Error (msg, expl, fix)](#apidoc.element.errors.Http402Error.Http402Error)
1.  [function <span class="apidocSignatureSpan">errors.Http402Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http402Error.super_)

#### [module errors.Http402Error.prototype](#apidoc.module.errors.Http402Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http402Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http402Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http402Error.prototype.</span>toString ()](#apidoc.element.errors.Http402Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http402Error.prototype.</span>name

#### [module errors.Http403Error](#apidoc.module.errors.Http403Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http403Error (msg, expl, fix)](#apidoc.element.errors.Http403Error.Http403Error)
1.  [function <span class="apidocSignatureSpan">errors.Http403Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http403Error.super_)

#### [module errors.Http403Error.prototype](#apidoc.module.errors.Http403Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http403Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http403Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http403Error.prototype.</span>toString ()](#apidoc.element.errors.Http403Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http403Error.prototype.</span>name

#### [module errors.Http404Error](#apidoc.module.errors.Http404Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http404Error (msg, expl, fix)](#apidoc.element.errors.Http404Error.Http404Error)
1.  [function <span class="apidocSignatureSpan">errors.Http404Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http404Error.super_)

#### [module errors.Http404Error.prototype](#apidoc.module.errors.Http404Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http404Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http404Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http404Error.prototype.</span>toString ()](#apidoc.element.errors.Http404Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http404Error.prototype.</span>name

#### [module errors.Http405Error](#apidoc.module.errors.Http405Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http405Error (msg, expl, fix)](#apidoc.element.errors.Http405Error.Http405Error)
1.  [function <span class="apidocSignatureSpan">errors.Http405Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http405Error.super_)

#### [module errors.Http405Error.prototype](#apidoc.module.errors.Http405Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http405Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http405Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http405Error.prototype.</span>toString ()](#apidoc.element.errors.Http405Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http405Error.prototype.</span>name

#### [module errors.Http406Error](#apidoc.module.errors.Http406Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http406Error (msg, expl, fix)](#apidoc.element.errors.Http406Error.Http406Error)
1.  [function <span class="apidocSignatureSpan">errors.Http406Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http406Error.super_)

#### [module errors.Http406Error.prototype](#apidoc.module.errors.Http406Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http406Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http406Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http406Error.prototype.</span>toString ()](#apidoc.element.errors.Http406Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http406Error.prototype.</span>name

#### [module errors.Http407Error](#apidoc.module.errors.Http407Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http407Error (msg, expl, fix)](#apidoc.element.errors.Http407Error.Http407Error)
1.  [function <span class="apidocSignatureSpan">errors.Http407Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http407Error.super_)

#### [module errors.Http407Error.prototype](#apidoc.module.errors.Http407Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http407Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http407Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http407Error.prototype.</span>toString ()](#apidoc.element.errors.Http407Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http407Error.prototype.</span>name

#### [module errors.Http408Error](#apidoc.module.errors.Http408Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http408Error (msg, expl, fix)](#apidoc.element.errors.Http408Error.Http408Error)
1.  [function <span class="apidocSignatureSpan">errors.Http408Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http408Error.super_)

#### [module errors.Http408Error.prototype](#apidoc.module.errors.Http408Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http408Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http408Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http408Error.prototype.</span>toString ()](#apidoc.element.errors.Http408Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http408Error.prototype.</span>name

#### [module errors.Http409Error](#apidoc.module.errors.Http409Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http409Error (msg, expl, fix)](#apidoc.element.errors.Http409Error.Http409Error)
1.  [function <span class="apidocSignatureSpan">errors.Http409Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http409Error.super_)

#### [module errors.Http409Error.prototype](#apidoc.module.errors.Http409Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http409Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http409Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http409Error.prototype.</span>toString ()](#apidoc.element.errors.Http409Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http409Error.prototype.</span>name

#### [module errors.Http410Error](#apidoc.module.errors.Http410Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http410Error (msg, expl, fix)](#apidoc.element.errors.Http410Error.Http410Error)
1.  [function <span class="apidocSignatureSpan">errors.Http410Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http410Error.super_)

#### [module errors.Http410Error.prototype](#apidoc.module.errors.Http410Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http410Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http410Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http410Error.prototype.</span>toString ()](#apidoc.element.errors.Http410Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http410Error.prototype.</span>name

#### [module errors.Http411Error](#apidoc.module.errors.Http411Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http411Error (msg, expl, fix)](#apidoc.element.errors.Http411Error.Http411Error)
1.  [function <span class="apidocSignatureSpan">errors.Http411Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http411Error.super_)

#### [module errors.Http411Error.prototype](#apidoc.module.errors.Http411Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http411Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http411Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http411Error.prototype.</span>toString ()](#apidoc.element.errors.Http411Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http411Error.prototype.</span>name

#### [module errors.Http412Error](#apidoc.module.errors.Http412Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http412Error (msg, expl, fix)](#apidoc.element.errors.Http412Error.Http412Error)
1.  [function <span class="apidocSignatureSpan">errors.Http412Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http412Error.super_)

#### [module errors.Http412Error.prototype](#apidoc.module.errors.Http412Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http412Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http412Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http412Error.prototype.</span>toString ()](#apidoc.element.errors.Http412Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http412Error.prototype.</span>name

#### [module errors.Http413Error](#apidoc.module.errors.Http413Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http413Error (msg, expl, fix)](#apidoc.element.errors.Http413Error.Http413Error)
1.  [function <span class="apidocSignatureSpan">errors.Http413Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http413Error.super_)

#### [module errors.Http413Error.prototype](#apidoc.module.errors.Http413Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http413Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http413Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http413Error.prototype.</span>toString ()](#apidoc.element.errors.Http413Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http413Error.prototype.</span>name

#### [module errors.Http414Error](#apidoc.module.errors.Http414Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http414Error (msg, expl, fix)](#apidoc.element.errors.Http414Error.Http414Error)
1.  [function <span class="apidocSignatureSpan">errors.Http414Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http414Error.super_)

#### [module errors.Http414Error.prototype](#apidoc.module.errors.Http414Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http414Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http414Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http414Error.prototype.</span>toString ()](#apidoc.element.errors.Http414Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http414Error.prototype.</span>name

#### [module errors.Http415Error](#apidoc.module.errors.Http415Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http415Error (msg, expl, fix)](#apidoc.element.errors.Http415Error.Http415Error)
1.  [function <span class="apidocSignatureSpan">errors.Http415Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http415Error.super_)

#### [module errors.Http415Error.prototype](#apidoc.module.errors.Http415Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http415Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http415Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http415Error.prototype.</span>toString ()](#apidoc.element.errors.Http415Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http415Error.prototype.</span>name

#### [module errors.Http416Error](#apidoc.module.errors.Http416Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http416Error (msg, expl, fix)](#apidoc.element.errors.Http416Error.Http416Error)
1.  [function <span class="apidocSignatureSpan">errors.Http416Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http416Error.super_)

#### [module errors.Http416Error.prototype](#apidoc.module.errors.Http416Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http416Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http416Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http416Error.prototype.</span>toString ()](#apidoc.element.errors.Http416Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http416Error.prototype.</span>name

#### [module errors.Http417Error](#apidoc.module.errors.Http417Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http417Error (msg, expl, fix)](#apidoc.element.errors.Http417Error.Http417Error)
1.  [function <span class="apidocSignatureSpan">errors.Http417Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http417Error.super_)

#### [module errors.Http417Error.prototype](#apidoc.module.errors.Http417Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http417Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http417Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http417Error.prototype.</span>toString ()](#apidoc.element.errors.Http417Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http417Error.prototype.</span>name

#### [module errors.Http418Error](#apidoc.module.errors.Http418Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http418Error (msg, expl, fix)](#apidoc.element.errors.Http418Error.Http418Error)
1.  [function <span class="apidocSignatureSpan">errors.Http418Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http418Error.super_)

#### [module errors.Http418Error.prototype](#apidoc.module.errors.Http418Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http418Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http418Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http418Error.prototype.</span>toString ()](#apidoc.element.errors.Http418Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http418Error.prototype.</span>name

#### [module errors.Http421Error](#apidoc.module.errors.Http421Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http421Error (msg, expl, fix)](#apidoc.element.errors.Http421Error.Http421Error)
1.  [function <span class="apidocSignatureSpan">errors.Http421Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http421Error.super_)

#### [module errors.Http421Error.prototype](#apidoc.module.errors.Http421Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http421Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http421Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http421Error.prototype.</span>toString ()](#apidoc.element.errors.Http421Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http421Error.prototype.</span>name

#### [module errors.Http422Error](#apidoc.module.errors.Http422Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http422Error (msg, expl, fix)](#apidoc.element.errors.Http422Error.Http422Error)
1.  [function <span class="apidocSignatureSpan">errors.Http422Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http422Error.super_)

#### [module errors.Http422Error.prototype](#apidoc.module.errors.Http422Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http422Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http422Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http422Error.prototype.</span>toString ()](#apidoc.element.errors.Http422Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http422Error.prototype.</span>name

#### [module errors.Http423Error](#apidoc.module.errors.Http423Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http423Error (msg, expl, fix)](#apidoc.element.errors.Http423Error.Http423Error)
1.  [function <span class="apidocSignatureSpan">errors.Http423Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http423Error.super_)

#### [module errors.Http423Error.prototype](#apidoc.module.errors.Http423Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http423Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http423Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http423Error.prototype.</span>toString ()](#apidoc.element.errors.Http423Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http423Error.prototype.</span>name

#### [module errors.Http424Error](#apidoc.module.errors.Http424Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http424Error (msg, expl, fix)](#apidoc.element.errors.Http424Error.Http424Error)
1.  [function <span class="apidocSignatureSpan">errors.Http424Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http424Error.super_)

#### [module errors.Http424Error.prototype](#apidoc.module.errors.Http424Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http424Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http424Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http424Error.prototype.</span>toString ()](#apidoc.element.errors.Http424Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http424Error.prototype.</span>name

#### [module errors.Http425Error](#apidoc.module.errors.Http425Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http425Error (msg, expl, fix)](#apidoc.element.errors.Http425Error.Http425Error)
1.  [function <span class="apidocSignatureSpan">errors.Http425Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http425Error.super_)

#### [module errors.Http425Error.prototype](#apidoc.module.errors.Http425Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http425Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http425Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http425Error.prototype.</span>toString ()](#apidoc.element.errors.Http425Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http425Error.prototype.</span>name

#### [module errors.Http426Error](#apidoc.module.errors.Http426Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http426Error (msg, expl, fix)](#apidoc.element.errors.Http426Error.Http426Error)
1.  [function <span class="apidocSignatureSpan">errors.Http426Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http426Error.super_)

#### [module errors.Http426Error.prototype](#apidoc.module.errors.Http426Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http426Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http426Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http426Error.prototype.</span>toString ()](#apidoc.element.errors.Http426Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http426Error.prototype.</span>name

#### [module errors.Http428Error](#apidoc.module.errors.Http428Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http428Error (msg, expl, fix)](#apidoc.element.errors.Http428Error.Http428Error)
1.  [function <span class="apidocSignatureSpan">errors.Http428Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http428Error.super_)

#### [module errors.Http428Error.prototype](#apidoc.module.errors.Http428Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http428Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http428Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http428Error.prototype.</span>toString ()](#apidoc.element.errors.Http428Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http428Error.prototype.</span>name

#### [module errors.Http429Error](#apidoc.module.errors.Http429Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http429Error (msg, expl, fix)](#apidoc.element.errors.Http429Error.Http429Error)
1.  [function <span class="apidocSignatureSpan">errors.Http429Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http429Error.super_)

#### [module errors.Http429Error.prototype](#apidoc.module.errors.Http429Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http429Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http429Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http429Error.prototype.</span>toString ()](#apidoc.element.errors.Http429Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http429Error.prototype.</span>name

#### [module errors.Http431Error](#apidoc.module.errors.Http431Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http431Error (msg, expl, fix)](#apidoc.element.errors.Http431Error.Http431Error)
1.  [function <span class="apidocSignatureSpan">errors.Http431Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http431Error.super_)

#### [module errors.Http431Error.prototype](#apidoc.module.errors.Http431Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http431Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http431Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http431Error.prototype.</span>toString ()](#apidoc.element.errors.Http431Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http431Error.prototype.</span>name

#### [module errors.Http451Error](#apidoc.module.errors.Http451Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http451Error (msg, expl, fix)](#apidoc.element.errors.Http451Error.Http451Error)
1.  [function <span class="apidocSignatureSpan">errors.Http451Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http451Error.super_)

#### [module errors.Http451Error.prototype](#apidoc.module.errors.Http451Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http451Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http451Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http451Error.prototype.</span>toString ()](#apidoc.element.errors.Http451Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http451Error.prototype.</span>name

#### [module errors.Http500Error](#apidoc.module.errors.Http500Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http500Error (msg, expl, fix)](#apidoc.element.errors.Http500Error.Http500Error)
1.  [function <span class="apidocSignatureSpan">errors.Http500Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http500Error.super_)

#### [module errors.Http500Error.prototype](#apidoc.module.errors.Http500Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http500Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http500Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http500Error.prototype.</span>toString ()](#apidoc.element.errors.Http500Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http500Error.prototype.</span>name

#### [module errors.Http501Error](#apidoc.module.errors.Http501Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http501Error (msg, expl, fix)](#apidoc.element.errors.Http501Error.Http501Error)
1.  [function <span class="apidocSignatureSpan">errors.Http501Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http501Error.super_)

#### [module errors.Http501Error.prototype](#apidoc.module.errors.Http501Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http501Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http501Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http501Error.prototype.</span>toString ()](#apidoc.element.errors.Http501Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http501Error.prototype.</span>name

#### [module errors.Http502Error](#apidoc.module.errors.Http502Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http502Error (msg, expl, fix)](#apidoc.element.errors.Http502Error.Http502Error)
1.  [function <span class="apidocSignatureSpan">errors.Http502Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http502Error.super_)

#### [module errors.Http502Error.prototype](#apidoc.module.errors.Http502Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http502Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http502Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http502Error.prototype.</span>toString ()](#apidoc.element.errors.Http502Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http502Error.prototype.</span>name

#### [module errors.Http503Error](#apidoc.module.errors.Http503Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http503Error (msg, expl, fix)](#apidoc.element.errors.Http503Error.Http503Error)
1.  [function <span class="apidocSignatureSpan">errors.Http503Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http503Error.super_)

#### [module errors.Http503Error.prototype](#apidoc.module.errors.Http503Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http503Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http503Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http503Error.prototype.</span>toString ()](#apidoc.element.errors.Http503Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http503Error.prototype.</span>name

#### [module errors.Http504Error](#apidoc.module.errors.Http504Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http504Error (msg, expl, fix)](#apidoc.element.errors.Http504Error.Http504Error)
1.  [function <span class="apidocSignatureSpan">errors.Http504Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http504Error.super_)

#### [module errors.Http504Error.prototype](#apidoc.module.errors.Http504Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http504Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http504Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http504Error.prototype.</span>toString ()](#apidoc.element.errors.Http504Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http504Error.prototype.</span>name

#### [module errors.Http505Error](#apidoc.module.errors.Http505Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http505Error (msg, expl, fix)](#apidoc.element.errors.Http505Error.Http505Error)
1.  [function <span class="apidocSignatureSpan">errors.Http505Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http505Error.super_)

#### [module errors.Http505Error.prototype](#apidoc.module.errors.Http505Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http505Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http505Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http505Error.prototype.</span>toString ()](#apidoc.element.errors.Http505Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http505Error.prototype.</span>name

#### [module errors.Http506Error](#apidoc.module.errors.Http506Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http506Error (msg, expl, fix)](#apidoc.element.errors.Http506Error.Http506Error)
1.  [function <span class="apidocSignatureSpan">errors.Http506Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http506Error.super_)

#### [module errors.Http506Error.prototype](#apidoc.module.errors.Http506Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http506Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http506Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http506Error.prototype.</span>toString ()](#apidoc.element.errors.Http506Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http506Error.prototype.</span>name

#### [module errors.Http507Error](#apidoc.module.errors.Http507Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http507Error (msg, expl, fix)](#apidoc.element.errors.Http507Error.Http507Error)
1.  [function <span class="apidocSignatureSpan">errors.Http507Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http507Error.super_)

#### [module errors.Http507Error.prototype](#apidoc.module.errors.Http507Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http507Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http507Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http507Error.prototype.</span>toString ()](#apidoc.element.errors.Http507Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http507Error.prototype.</span>name

#### [module errors.Http508Error](#apidoc.module.errors.Http508Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http508Error (msg, expl, fix)](#apidoc.element.errors.Http508Error.Http508Error)
1.  [function <span class="apidocSignatureSpan">errors.Http508Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http508Error.super_)

#### [module errors.Http508Error.prototype](#apidoc.module.errors.Http508Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http508Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http508Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http508Error.prototype.</span>toString ()](#apidoc.element.errors.Http508Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http508Error.prototype.</span>name

#### [module errors.Http509Error](#apidoc.module.errors.Http509Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http509Error (msg, expl, fix)](#apidoc.element.errors.Http509Error.Http509Error)
1.  [function <span class="apidocSignatureSpan">errors.Http509Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http509Error.super_)

#### [module errors.Http509Error.prototype](#apidoc.module.errors.Http509Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http509Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http509Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http509Error.prototype.</span>toString ()](#apidoc.element.errors.Http509Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http509Error.prototype.</span>name

#### [module errors.Http510Error](#apidoc.module.errors.Http510Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http510Error (msg, expl, fix)](#apidoc.element.errors.Http510Error.Http510Error)
1.  [function <span class="apidocSignatureSpan">errors.Http510Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http510Error.super_)

#### [module errors.Http510Error.prototype](#apidoc.module.errors.Http510Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http510Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http510Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http510Error.prototype.</span>toString ()](#apidoc.element.errors.Http510Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http510Error.prototype.</span>name

#### [module errors.Http511Error](#apidoc.module.errors.Http511Error)
1.  [function <span class="apidocSignatureSpan">errors.</span>Http511Error (msg, expl, fix)](#apidoc.element.errors.Http511Error.Http511Error)
1.  [function <span class="apidocSignatureSpan">errors.Http511Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http511Error.super_)

#### [module errors.Http511Error.prototype](#apidoc.module.errors.Http511Error.prototype)
1.  [function <span class="apidocSignatureSpan">errors.Http511Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http511Error.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.Http511Error.prototype.</span>toString ()](#apidoc.element.errors.Http511Error.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.Http511Error.prototype.</span>name

#### [module errors.HttpError](#apidoc.module.errors.HttpError)
1.  [function <span class="apidocSignatureSpan">errors.</span>HttpError (msg, expl, fix)](#apidoc.element.errors.HttpError.HttpError)
1.  [function <span class="apidocSignatureSpan">errors.HttpError.</span>super_ ()](#apidoc.element.errors.HttpError.super_)

#### [module errors.HttpError.prototype](#apidoc.module.errors.HttpError.prototype)
1.  [function <span class="apidocSignatureSpan">errors.HttpError.prototype.</span>toJSON ()](#apidoc.element.errors.HttpError.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">errors.HttpError.prototype.</span>toString ()](#apidoc.element.errors.HttpError.prototype.toString)
1.  string <span class="apidocSignatureSpan">errors.HttpError.prototype.</span>name

#### [module errors.HttpError.super_](#apidoc.module.errors.HttpError.super_)
1.  [function <span class="apidocSignatureSpan">errors.HttpError.</span>super_ ()](#apidoc.element.errors.HttpError.super_.super_)
1.  [function <span class="apidocSignatureSpan">errors.HttpError.super_.</span>captureStackTrace ()](#apidoc.element.errors.HttpError.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">errors.HttpError.super_.</span>stackTraceLimit

#### [module errors.JS_ERRORS](#apidoc.module.errors.JS_ERRORS)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>Error ()](#apidoc.element.errors.JS_ERRORS.Error)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>EvalError ()](#apidoc.element.errors.JS_ERRORS.EvalError)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>RangeError ()](#apidoc.element.errors.JS_ERRORS.RangeError)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>ReferenceError ()](#apidoc.element.errors.JS_ERRORS.ReferenceError)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>SyntaxError ()](#apidoc.element.errors.JS_ERRORS.SyntaxError)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>TypeError ()](#apidoc.element.errors.JS_ERRORS.TypeError)
1.  [function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>URIError ()](#apidoc.element.errors.JS_ERRORS.URIError)



# <a name="apidoc.module.errors"></a>[module errors](#apidoc.module.errors)

#### <a name="apidoc.element.errors.Http400Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http400Error (msg, expl, fix)](#apidoc.element.errors.Http400Error)
- description and source-code
```javascript
Http400Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
errors.mapper('RangeError', function(rangeError) {
    return new errors.Http412Error('Invalid range requested');
})
.mapper('ReferenceError', function(refError) {
    return new errors.Http424Error('Bad reference given');
})
.mapper('SyntaxError', function(syntaxError) {
    return new errors.Http400Error('Invalid syntax');
});

// ...

res.send(new RangeError());
// => 412 response as per mapper
...
```

#### <a name="apidoc.element.errors.Http401Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http401Error (msg, expl, fix)](#apidoc.element.errors.Http401Error)
- description and source-code
```javascript
Http401Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
Explanation: You do not have access to read /root/foo
Response: Request a file you have permissions to access

'''

Use the options style constructor to assign standard properties:
'''js
console.log(new errors.Http401Error({
	message: "Expired Token",
	explanation: "Your token has expired"}).toString());
'''

outputs:
'''
Http401Error: Expired Token
...
```

#### <a name="apidoc.element.errors.Http402Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http402Error (msg, expl, fix)](#apidoc.element.errors.Http402Error)
- description and source-code
```javascript
Http402Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http403Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http403Error (msg, expl, fix)](#apidoc.element.errors.Http403Error)
- description and source-code
```javascript
Http403Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http404Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http404Error (msg, expl, fix)](#apidoc.element.errors.Http404Error)
- description and source-code
```javascript
Http404Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
installed. If express is installed, errors automatically patches 'express''s
'response.send()' method to support 'send()'ing 'Error' based objects.

So the following is valid:
'''js
app.get('/users/:user', function(req, res) {
    users.get(req.params.user, function(err, user) {
        return res.send(err || user || new errors.Http404Error('User does not exist'));
    });
});
'''

By default both vanilla errors (those provided by the JS runtime) and errors
which have a 'code' which is not a valid HTTP status code are mapped to a '500'
response.
...
```

#### <a name="apidoc.element.errors.Http405Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http405Error (msg, expl, fix)](#apidoc.element.errors.Http405Error)
- description and source-code
```javascript
Http405Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http406Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http406Error (msg, expl, fix)](#apidoc.element.errors.Http406Error)
- description and source-code
```javascript
Http406Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http407Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http407Error (msg, expl, fix)](#apidoc.element.errors.Http407Error)
- description and source-code
```javascript
Http407Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http408Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http408Error (msg, expl, fix)](#apidoc.element.errors.Http408Error)
- description and source-code
```javascript
Http408Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http409Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http409Error (msg, expl, fix)](#apidoc.element.errors.Http409Error)
- description and source-code
```javascript
Http409Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http410Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http410Error (msg, expl, fix)](#apidoc.element.errors.Http410Error)
- description and source-code
```javascript
Http410Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http411Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http411Error (msg, expl, fix)](#apidoc.element.errors.Http411Error)
- description and source-code
```javascript
Http411Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http412Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http412Error (msg, expl, fix)](#apidoc.element.errors.Http412Error)
- description and source-code
```javascript
Http412Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
both will result in a '500' response.

Mappers can also be used with 'express''s 'send()' method.

For example:
'''js
errors.mapper('RangeError', function(rangeError) {
    return new errors.Http412Error('Invalid range requested');
})
.mapper('ReferenceError', function(refError) {
    return new errors.Http424Error('Bad reference given');
})
.mapper('SyntaxError', function(syntaxError) {
    return new errors.Http400Error('Invalid syntax');
});
...
```

#### <a name="apidoc.element.errors.Http413Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http413Error (msg, expl, fix)](#apidoc.element.errors.Http413Error)
- description and source-code
```javascript
Http413Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
like 'toString()' and 'toJSON()' return representation without stack
traces. You can enable stack traces by leveraging the 'errors.stacks()'
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.
...
```

#### <a name="apidoc.element.errors.Http414Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http414Error (msg, expl, fix)](#apidoc.element.errors.Http414Error)
- description and source-code
```javascript
Http414Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http415Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http415Error (msg, expl, fix)](#apidoc.element.errors.Http415Error)
- description and source-code
```javascript
Http415Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http416Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http416Error (msg, expl, fix)](#apidoc.element.errors.Http416Error)
- description and source-code
```javascript
Http416Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http417Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http417Error (msg, expl, fix)](#apidoc.element.errors.Http417Error)
- description and source-code
```javascript
Http417Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http418Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http418Error (msg, expl, fix)](#apidoc.element.errors.Http418Error)
- description and source-code
```javascript
Http418Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http421Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http421Error (msg, expl, fix)](#apidoc.element.errors.Http421Error)
- description and source-code
```javascript
Http421Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http422Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http422Error (msg, expl, fix)](#apidoc.element.errors.Http422Error)
- description and source-code
```javascript
Http422Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http423Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http423Error (msg, expl, fix)](#apidoc.element.errors.Http423Error)
- description and source-code
```javascript
Http423Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http424Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http424Error (msg, expl, fix)](#apidoc.element.errors.Http424Error)
- description and source-code
```javascript
Http424Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...

For example:
'''js
errors.mapper('RangeError', function(rangeError) {
    return new errors.Http412Error('Invalid range requested');
})
.mapper('ReferenceError', function(refError) {
    return new errors.Http424Error('Bad reference given');
})
.mapper('SyntaxError', function(syntaxError) {
    return new errors.Http400Error('Invalid syntax');
});

// ...
...
```

#### <a name="apidoc.element.errors.Http425Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http425Error (msg, expl, fix)](#apidoc.element.errors.Http425Error)
- description and source-code
```javascript
Http425Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http426Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http426Error (msg, expl, fix)](#apidoc.element.errors.Http426Error)
- description and source-code
```javascript
Http426Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http428Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http428Error (msg, expl, fix)](#apidoc.element.errors.Http428Error)
- description and source-code
```javascript
Http428Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http429Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http429Error (msg, expl, fix)](#apidoc.element.errors.Http429Error)
- description and source-code
```javascript
Http429Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http431Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http431Error (msg, expl, fix)](#apidoc.element.errors.Http431Error)
- description and source-code
```javascript
Http431Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http451Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http451Error (msg, expl, fix)](#apidoc.element.errors.Http451Error)
- description and source-code
```javascript
Http451Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http500Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http500Error (msg, expl, fix)](#apidoc.element.errors.Http500Error)
- description and source-code
```javascript
Http500Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
naming convention 'Http[code]Error'. For example 'Http401Error' and
'Http500Error' which have a code of '401' and '500' respectively.

For example to leverage the HTTP errors:
'''js
throw new errors.Http401Error();
// ...
throw new errors.Http500Error('Something bad happened');
'''

## Connect/Express middleware integration

**Compatibility**
Errors version 0.1.0 only works with Express < 4.0.0.
...
```

#### <a name="apidoc.element.errors.Http501Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http501Error (msg, expl, fix)](#apidoc.element.errors.Http501Error)
- description and source-code
```javascript
Http501Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http502Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http502Error (msg, expl, fix)](#apidoc.element.errors.Http502Error)
- description and source-code
```javascript
Http502Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http503Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http503Error (msg, expl, fix)](#apidoc.element.errors.Http503Error)
- description and source-code
```javascript
Http503Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http504Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http504Error (msg, expl, fix)](#apidoc.element.errors.Http504Error)
- description and source-code
```javascript
Http504Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http505Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http505Error (msg, expl, fix)](#apidoc.element.errors.Http505Error)
- description and source-code
```javascript
Http505Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http506Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http506Error (msg, expl, fix)](#apidoc.element.errors.Http506Error)
- description and source-code
```javascript
Http506Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http507Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http507Error (msg, expl, fix)](#apidoc.element.errors.Http507Error)
- description and source-code
```javascript
Http507Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http508Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http508Error (msg, expl, fix)](#apidoc.element.errors.Http508Error)
- description and source-code
```javascript
Http508Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http509Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http509Error (msg, expl, fix)](#apidoc.element.errors.Http509Error)
- description and source-code
```javascript
Http509Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http510Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http510Error (msg, expl, fix)](#apidoc.element.errors.Http510Error)
- description and source-code
```javascript
Http510Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http511Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http511Error (msg, expl, fix)](#apidoc.element.errors.Http511Error)
- description and source-code
```javascript
Http511Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.HttpError"></a>[function <span class="apidocSignatureSpan">errors.</span>HttpError (msg, expl, fix)](#apidoc.element.errors.HttpError)
- description and source-code
```javascript
HttpError = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.HttpError.super_"></a>[function <span class="apidocSignatureSpan">errors.</span>HttpError.super_ ()](#apidoc.element.errors.HttpError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.create"></a>[function <span class="apidocSignatureSpan">errors.</span>create (options)](#apidoc.element.errors.create)
- description and source-code
```javascript
create = function (options) {
    var options = options || {}
        , scope = options.scope || exports
        , parent = options.parent || Error
        , defaultMessage = options.defaultMessage
            || 'An unexpected ' + options.name + ' occurred.'
        , className = options.name
        , errorCode = options.code || nextCode()
        , statusCode = options.status
        , defaultExplanation = options.defaultExplanation
        , defaultResponse = options.defaultResponse
        , formattedStack
        , stack = {};


<span class="apidocCodeCommentSpan">/**
 * Create a new instance of the exception which accepts
 * 2 forms of parameters.
 *
 * (a) Passing the message, explanation and response
 * as individual argument strings:
 * Create a new instance of the exception optionally
 * specifying a message, explanation and response
 * for the new instance. If any of the arguments are
 * null, their value will default to their respective
 * default value use on the 'create' call, or will
 * be null if no default was specified.
 *
 * (b) Passing an options style object which contains
 * key / value pairs. In this form keys map to the
 * attributes of the error object. Note that the properties
 * 'stack', 'name' and 'code' cannot be set via the options
 * style object in this form.
 *
 * @param {String|Object} msg The message to use for the error.
 * @param {String} expl The explanation to use for the error.
 * @param {String} fix The response to use for the error.
 * @return {Object} The newly created error.
 */
</span>
    scope[className] = function(msg, expl, fix) {
    	var attrs = {};
    	if (typeof msg !== null && typeof msg === 'object') {
    		attrs = msg;
    		msg = attrs['message'] || defaultMessage;
    		if (attrs.hasOwnProperty('stack')
    				|| attrs.hasOwnProperty('name')
    				|| attrs.hasOwnProperty('code')) {
    			throw Error("Properties 'stack', 'name' or 'code' " +
    					"cannot be overridden");
    		}
    	}
    	attrs['status'] = attrs['status'] || statusCode;
        msg = msg || defaultMessage;
        expl = expl || defaultExplanation;
        fix = fix || defaultResponse;

        parent.call(this, msg);

        // hack around the defineProperty for stack so
        // we can delay stack formatting until access
        // for performance reasons
        Error.captureStackTrace(stack, scope[className]);

/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
        Object.defineProperty(this, 'stack', {
            configurable: true,
            enumerable: false,
            get: function() {
                if (!formattedStack) {
                    formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
                }
                return formattedStack;
            }
        });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

        Object.defineProperty(this, 'explanation', {
            value: attrs['explanation'] || expl,
            configurable: true,
            enumerable: true
        });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

        Object.defineProperty(this, 'response', {
            value: attrs['response'] || fix,
            configurable: true,
            enumerable: true
        });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

        Object.defineProperty(this, 'code', {
            value: attrs['code'] || errorCode,
            configurable: true,
            enumerable: true
        });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

        Object.defineProperty(this, 'status', {
            value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
            configurable: true,
            // normalize for http status code and connect compat
            enumerable: true
        });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

        Obje ...
```
- example usage
```shell
...
require('errors');
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
...
```

#### <a name="apidoc.element.errors.errorToJSON"></a>[function <span class="apidocSignatureSpan">errors.</span>errorToJSON (err, attrMap)](#apidoc.element.errors.errorToJSON)
- description and source-code
```javascript
errorToJSON = function (err, attrMap) {
	var attrs = attrMap || _DEFAULT_ERROR_MAPPING,
		formatted = {};

	for (var dest in attrs) {
		for (var attr_index in attrs[dest]) {
			var val = err,
				src = attrs[dest][attr_index],
				segs = src.split('.');
			for (var seg_index in segs) {
				if (segs[seg_index] == 'stack' && !useStack) {
					val = null;
					break;
				}
				val = segs[seg_index] in val ? val[segs[seg_index]] : null;
			}
			if (val != null) {
				formatted[dest] = val;
			}
		}
	}
	return formatted;
}
```
- example usage
```shell
...
'''

## Native errors

Often times you need to extract 'errors-like' properties from native error
objects. For example you have a native JS or node error and you want to
extract it's errors-like properties. An error's module-level function
called 'errors.errorToJSON()' allows you to do this.

For example to extract error properties from a native error ('errors.stacks'
is set to 'false' in this example):
'''js
console.log("%j", errors.errorToJSON(new TypeError("Bad type")));
'''
...
```

#### <a name="apidoc.element.errors.find"></a>[function <span class="apidocSignatureSpan">errors.</span>find (err)](#apidoc.element.errors.find)
- description and source-code
```javascript
find = function (err) {
    return (typeof err == 'number') ? codes[err] : names[err];
}
```
- example usage
```shell
...

For convenience, errors keeps track of all the errors you've defined
via the errors module and allows you to look them up via 'name' or
'code'.

So from our previous example:
'''js
errors.find(1100);
errors.find('SecurityError')
'''

Will both return the 'SecutiryError' we defined.

## Stack traces
...
```

#### <a name="apidoc.element.errors.isError"></a>[function <span class="apidocSignatureSpan">errors.</span>isError (err)](#apidoc.element.errors.isError)
- description and source-code
```javascript
function isError(err) {
    return err && err.hasOwnProperty('explanation') && err.hasOwnProperty('code');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.mapError"></a>[function <span class="apidocSignatureSpan">errors.</span>mapError (err)](#apidoc.element.errors.mapError)
- description and source-code
```javascript
mapError = function (err) {
    return mapper(err.name) ? mapper(err.name)(err) : err;
}
```
- example usage
```shell
...
'''js
// mappers
errors.create({name: 'InvalidUsernameError'});
errors.create({name: 'InvalidPasswordError'});
errors.mapper(['InvalidUsernameError', 'InvalidPasswordError'], function(err) {
    return new errors.SecurityError('Invalid credentials supplied');
});
console.log(errors.mapError(new errors.InvalidUsernameError()).toString());
console.log(errors.mapError(new errors.InvalidPasswordError()).toString());
'''

outputs:
'''
SecurityError: Invalid credentials supplied
Code: 1100
...
```

#### <a name="apidoc.element.errors.mapper"></a>[function <span class="apidocSignatureSpan">errors.</span>mapper (errName, fn)](#apidoc.element.errors.mapper)
- description and source-code
```javascript
mapper = function (errName, fn) {
    if (arguments.length == 2) {
        asArray(errName).forEach(function(name) {
            mappers[name] = fn;
        });
        return exports;
    }
    return mappers[errName];
}
```
- example usage
```shell
...

For example if you wanted to mask invalid user and password errors into
a generic credentials error:
'''js
// mappers
errors.create({name: 'InvalidUsernameError'});
errors.create({name: 'InvalidPasswordError'});
errors.mapper(['InvalidUsernameError', 'InvalidPasswordError'], function(err) {
    return new errors.SecurityError('Invalid credentials supplied');
});
console.log(errors.mapError(new errors.InvalidUsernameError()).toString());
console.log(errors.mapError(new errors.InvalidPasswordError()).toString());
'''

outputs:
...
```

#### <a name="apidoc.element.errors.stacks"></a>[function <span class="apidocSignatureSpan">errors.</span>stacks (useStacks)](#apidoc.element.errors.stacks)
- description and source-code
```javascript
stacks = function (useStacks) {
    if (useStacks == null || useStacks == undefined) {
        return useStack;
    }
    useStack = useStacks;
}
```
- example usage
```shell
...

Will both return the 'SecutiryError' we defined.

## Stack traces

By default stack traces are disabled which means that error methods
like 'toString()' and 'toJSON()' return representation without stack
traces. You can enable stack traces by leveraging the 'errors.stacks()'
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
...
```

#### <a name="apidoc.element.errors.title"></a>[function <span class="apidocSignatureSpan">errors.</span>title (title)](#apidoc.element.errors.title)
- description and source-code
```javascript
title = function (title) {
    if (title == null || title == undefined) {
        return pageTitle;
    }
    pageTitle = title;
}
```
- example usage
```shell
...
    "message": "An unexpected DatabaseConnectionError occurred."
}
'''

For HTML based responses, 'send()'ing an error will produce a HTML
response that looks like express's or connect's 'errorHandler()' middleware.
That is, it's an HTML page with minimal styling. Moreover you can control
the HTML response page title using the 'errors.title('My Title')' method.
You can also control if stack traces should be included in the 'send()' by
using the 'errors.stacks()' method.

## License

(The MIT License)
...
```



# <a name="apidoc.module.errors.Http400Error"></a>[module errors.Http400Error](#apidoc.module.errors.Http400Error)

#### <a name="apidoc.element.errors.Http400Error.Http400Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http400Error (msg, expl, fix)](#apidoc.element.errors.Http400Error.Http400Error)
- description and source-code
```javascript
Http400Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
errors.mapper('RangeError', function(rangeError) {
    return new errors.Http412Error('Invalid range requested');
})
.mapper('ReferenceError', function(refError) {
    return new errors.Http424Error('Bad reference given');
})
.mapper('SyntaxError', function(syntaxError) {
    return new errors.Http400Error('Invalid syntax');
});

// ...

res.send(new RangeError());
// => 412 response as per mapper
...
```

#### <a name="apidoc.element.errors.Http400Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http400Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http400Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http400Error.prototype"></a>[module errors.Http400Error.prototype](#apidoc.module.errors.Http400Error.prototype)

#### <a name="apidoc.element.errors.Http400Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http400Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http400Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http400Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http400Error.prototype.</span>toString ()](#apidoc.element.errors.Http400Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http401Error"></a>[module errors.Http401Error](#apidoc.module.errors.Http401Error)

#### <a name="apidoc.element.errors.Http401Error.Http401Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http401Error (msg, expl, fix)](#apidoc.element.errors.Http401Error.Http401Error)
- description and source-code
```javascript
Http401Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
Explanation: You do not have access to read /root/foo
Response: Request a file you have permissions to access

'''

Use the options style constructor to assign standard properties:
'''js
console.log(new errors.Http401Error({
	message: "Expired Token",
	explanation: "Your token has expired"}).toString());
'''

outputs:
'''
Http401Error: Expired Token
...
```

#### <a name="apidoc.element.errors.Http401Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http401Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http401Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http401Error.prototype"></a>[module errors.Http401Error.prototype](#apidoc.module.errors.Http401Error.prototype)

#### <a name="apidoc.element.errors.Http401Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http401Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http401Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http401Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http401Error.prototype.</span>toString ()](#apidoc.element.errors.Http401Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http402Error"></a>[module errors.Http402Error](#apidoc.module.errors.Http402Error)

#### <a name="apidoc.element.errors.Http402Error.Http402Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http402Error (msg, expl, fix)](#apidoc.element.errors.Http402Error.Http402Error)
- description and source-code
```javascript
Http402Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http402Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http402Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http402Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http402Error.prototype"></a>[module errors.Http402Error.prototype](#apidoc.module.errors.Http402Error.prototype)

#### <a name="apidoc.element.errors.Http402Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http402Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http402Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http402Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http402Error.prototype.</span>toString ()](#apidoc.element.errors.Http402Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http403Error"></a>[module errors.Http403Error](#apidoc.module.errors.Http403Error)

#### <a name="apidoc.element.errors.Http403Error.Http403Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http403Error (msg, expl, fix)](#apidoc.element.errors.Http403Error.Http403Error)
- description and source-code
```javascript
Http403Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http403Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http403Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http403Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http403Error.prototype"></a>[module errors.Http403Error.prototype](#apidoc.module.errors.Http403Error.prototype)

#### <a name="apidoc.element.errors.Http403Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http403Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http403Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http403Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http403Error.prototype.</span>toString ()](#apidoc.element.errors.Http403Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http404Error"></a>[module errors.Http404Error](#apidoc.module.errors.Http404Error)

#### <a name="apidoc.element.errors.Http404Error.Http404Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http404Error (msg, expl, fix)](#apidoc.element.errors.Http404Error.Http404Error)
- description and source-code
```javascript
Http404Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
installed. If express is installed, errors automatically patches 'express''s
'response.send()' method to support 'send()'ing 'Error' based objects.

So the following is valid:
'''js
app.get('/users/:user', function(req, res) {
    users.get(req.params.user, function(err, user) {
        return res.send(err || user || new errors.Http404Error('User does not exist'));
    });
});
'''

By default both vanilla errors (those provided by the JS runtime) and errors
which have a 'code' which is not a valid HTTP status code are mapped to a '500'
response.
...
```

#### <a name="apidoc.element.errors.Http404Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http404Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http404Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http404Error.prototype"></a>[module errors.Http404Error.prototype](#apidoc.module.errors.Http404Error.prototype)

#### <a name="apidoc.element.errors.Http404Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http404Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http404Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http404Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http404Error.prototype.</span>toString ()](#apidoc.element.errors.Http404Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http405Error"></a>[module errors.Http405Error](#apidoc.module.errors.Http405Error)

#### <a name="apidoc.element.errors.Http405Error.Http405Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http405Error (msg, expl, fix)](#apidoc.element.errors.Http405Error.Http405Error)
- description and source-code
```javascript
Http405Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http405Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http405Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http405Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http405Error.prototype"></a>[module errors.Http405Error.prototype](#apidoc.module.errors.Http405Error.prototype)

#### <a name="apidoc.element.errors.Http405Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http405Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http405Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http405Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http405Error.prototype.</span>toString ()](#apidoc.element.errors.Http405Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http406Error"></a>[module errors.Http406Error](#apidoc.module.errors.Http406Error)

#### <a name="apidoc.element.errors.Http406Error.Http406Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http406Error (msg, expl, fix)](#apidoc.element.errors.Http406Error.Http406Error)
- description and source-code
```javascript
Http406Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http406Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http406Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http406Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http406Error.prototype"></a>[module errors.Http406Error.prototype](#apidoc.module.errors.Http406Error.prototype)

#### <a name="apidoc.element.errors.Http406Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http406Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http406Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http406Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http406Error.prototype.</span>toString ()](#apidoc.element.errors.Http406Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http407Error"></a>[module errors.Http407Error](#apidoc.module.errors.Http407Error)

#### <a name="apidoc.element.errors.Http407Error.Http407Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http407Error (msg, expl, fix)](#apidoc.element.errors.Http407Error.Http407Error)
- description and source-code
```javascript
Http407Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http407Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http407Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http407Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http407Error.prototype"></a>[module errors.Http407Error.prototype](#apidoc.module.errors.Http407Error.prototype)

#### <a name="apidoc.element.errors.Http407Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http407Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http407Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http407Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http407Error.prototype.</span>toString ()](#apidoc.element.errors.Http407Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http408Error"></a>[module errors.Http408Error](#apidoc.module.errors.Http408Error)

#### <a name="apidoc.element.errors.Http408Error.Http408Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http408Error (msg, expl, fix)](#apidoc.element.errors.Http408Error.Http408Error)
- description and source-code
```javascript
Http408Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http408Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http408Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http408Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http408Error.prototype"></a>[module errors.Http408Error.prototype](#apidoc.module.errors.Http408Error.prototype)

#### <a name="apidoc.element.errors.Http408Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http408Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http408Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http408Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http408Error.prototype.</span>toString ()](#apidoc.element.errors.Http408Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http409Error"></a>[module errors.Http409Error](#apidoc.module.errors.Http409Error)

#### <a name="apidoc.element.errors.Http409Error.Http409Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http409Error (msg, expl, fix)](#apidoc.element.errors.Http409Error.Http409Error)
- description and source-code
```javascript
Http409Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http409Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http409Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http409Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http409Error.prototype"></a>[module errors.Http409Error.prototype](#apidoc.module.errors.Http409Error.prototype)

#### <a name="apidoc.element.errors.Http409Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http409Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http409Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http409Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http409Error.prototype.</span>toString ()](#apidoc.element.errors.Http409Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http410Error"></a>[module errors.Http410Error](#apidoc.module.errors.Http410Error)

#### <a name="apidoc.element.errors.Http410Error.Http410Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http410Error (msg, expl, fix)](#apidoc.element.errors.Http410Error.Http410Error)
- description and source-code
```javascript
Http410Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http410Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http410Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http410Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http410Error.prototype"></a>[module errors.Http410Error.prototype](#apidoc.module.errors.Http410Error.prototype)

#### <a name="apidoc.element.errors.Http410Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http410Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http410Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http410Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http410Error.prototype.</span>toString ()](#apidoc.element.errors.Http410Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http411Error"></a>[module errors.Http411Error](#apidoc.module.errors.Http411Error)

#### <a name="apidoc.element.errors.Http411Error.Http411Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http411Error (msg, expl, fix)](#apidoc.element.errors.Http411Error.Http411Error)
- description and source-code
```javascript
Http411Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http411Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http411Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http411Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http411Error.prototype"></a>[module errors.Http411Error.prototype](#apidoc.module.errors.Http411Error.prototype)

#### <a name="apidoc.element.errors.Http411Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http411Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http411Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http411Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http411Error.prototype.</span>toString ()](#apidoc.element.errors.Http411Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http412Error"></a>[module errors.Http412Error](#apidoc.module.errors.Http412Error)

#### <a name="apidoc.element.errors.Http412Error.Http412Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http412Error (msg, expl, fix)](#apidoc.element.errors.Http412Error.Http412Error)
- description and source-code
```javascript
Http412Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
both will result in a '500' response.

Mappers can also be used with 'express''s 'send()' method.

For example:
'''js
errors.mapper('RangeError', function(rangeError) {
    return new errors.Http412Error('Invalid range requested');
})
.mapper('ReferenceError', function(refError) {
    return new errors.Http424Error('Bad reference given');
})
.mapper('SyntaxError', function(syntaxError) {
    return new errors.Http400Error('Invalid syntax');
});
...
```

#### <a name="apidoc.element.errors.Http412Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http412Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http412Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http412Error.prototype"></a>[module errors.Http412Error.prototype](#apidoc.module.errors.Http412Error.prototype)

#### <a name="apidoc.element.errors.Http412Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http412Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http412Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http412Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http412Error.prototype.</span>toString ()](#apidoc.element.errors.Http412Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http413Error"></a>[module errors.Http413Error](#apidoc.module.errors.Http413Error)

#### <a name="apidoc.element.errors.Http413Error.Http413Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http413Error (msg, expl, fix)](#apidoc.element.errors.Http413Error.Http413Error)
- description and source-code
```javascript
Http413Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
like 'toString()' and 'toJSON()' return representation without stack
traces. You can enable stack traces by leveraging the 'errors.stacks()'
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.
...
```

#### <a name="apidoc.element.errors.Http413Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http413Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http413Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http413Error.prototype"></a>[module errors.Http413Error.prototype](#apidoc.module.errors.Http413Error.prototype)

#### <a name="apidoc.element.errors.Http413Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http413Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http413Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http413Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http413Error.prototype.</span>toString ()](#apidoc.element.errors.Http413Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http414Error"></a>[module errors.Http414Error](#apidoc.module.errors.Http414Error)

#### <a name="apidoc.element.errors.Http414Error.Http414Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http414Error (msg, expl, fix)](#apidoc.element.errors.Http414Error.Http414Error)
- description and source-code
```javascript
Http414Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http414Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http414Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http414Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http414Error.prototype"></a>[module errors.Http414Error.prototype](#apidoc.module.errors.Http414Error.prototype)

#### <a name="apidoc.element.errors.Http414Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http414Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http414Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http414Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http414Error.prototype.</span>toString ()](#apidoc.element.errors.Http414Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http415Error"></a>[module errors.Http415Error](#apidoc.module.errors.Http415Error)

#### <a name="apidoc.element.errors.Http415Error.Http415Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http415Error (msg, expl, fix)](#apidoc.element.errors.Http415Error.Http415Error)
- description and source-code
```javascript
Http415Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http415Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http415Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http415Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http415Error.prototype"></a>[module errors.Http415Error.prototype](#apidoc.module.errors.Http415Error.prototype)

#### <a name="apidoc.element.errors.Http415Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http415Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http415Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http415Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http415Error.prototype.</span>toString ()](#apidoc.element.errors.Http415Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http416Error"></a>[module errors.Http416Error](#apidoc.module.errors.Http416Error)

#### <a name="apidoc.element.errors.Http416Error.Http416Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http416Error (msg, expl, fix)](#apidoc.element.errors.Http416Error.Http416Error)
- description and source-code
```javascript
Http416Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http416Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http416Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http416Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http416Error.prototype"></a>[module errors.Http416Error.prototype](#apidoc.module.errors.Http416Error.prototype)

#### <a name="apidoc.element.errors.Http416Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http416Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http416Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http416Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http416Error.prototype.</span>toString ()](#apidoc.element.errors.Http416Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http417Error"></a>[module errors.Http417Error](#apidoc.module.errors.Http417Error)

#### <a name="apidoc.element.errors.Http417Error.Http417Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http417Error (msg, expl, fix)](#apidoc.element.errors.Http417Error.Http417Error)
- description and source-code
```javascript
Http417Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http417Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http417Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http417Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http417Error.prototype"></a>[module errors.Http417Error.prototype](#apidoc.module.errors.Http417Error.prototype)

#### <a name="apidoc.element.errors.Http417Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http417Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http417Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http417Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http417Error.prototype.</span>toString ()](#apidoc.element.errors.Http417Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http418Error"></a>[module errors.Http418Error](#apidoc.module.errors.Http418Error)

#### <a name="apidoc.element.errors.Http418Error.Http418Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http418Error (msg, expl, fix)](#apidoc.element.errors.Http418Error.Http418Error)
- description and source-code
```javascript
Http418Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http418Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http418Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http418Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http418Error.prototype"></a>[module errors.Http418Error.prototype](#apidoc.module.errors.Http418Error.prototype)

#### <a name="apidoc.element.errors.Http418Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http418Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http418Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http418Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http418Error.prototype.</span>toString ()](#apidoc.element.errors.Http418Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http421Error"></a>[module errors.Http421Error](#apidoc.module.errors.Http421Error)

#### <a name="apidoc.element.errors.Http421Error.Http421Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http421Error (msg, expl, fix)](#apidoc.element.errors.Http421Error.Http421Error)
- description and source-code
```javascript
Http421Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http421Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http421Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http421Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http421Error.prototype"></a>[module errors.Http421Error.prototype](#apidoc.module.errors.Http421Error.prototype)

#### <a name="apidoc.element.errors.Http421Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http421Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http421Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http421Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http421Error.prototype.</span>toString ()](#apidoc.element.errors.Http421Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http422Error"></a>[module errors.Http422Error](#apidoc.module.errors.Http422Error)

#### <a name="apidoc.element.errors.Http422Error.Http422Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http422Error (msg, expl, fix)](#apidoc.element.errors.Http422Error.Http422Error)
- description and source-code
```javascript
Http422Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http422Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http422Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http422Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http422Error.prototype"></a>[module errors.Http422Error.prototype](#apidoc.module.errors.Http422Error.prototype)

#### <a name="apidoc.element.errors.Http422Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http422Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http422Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http422Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http422Error.prototype.</span>toString ()](#apidoc.element.errors.Http422Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http423Error"></a>[module errors.Http423Error](#apidoc.module.errors.Http423Error)

#### <a name="apidoc.element.errors.Http423Error.Http423Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http423Error (msg, expl, fix)](#apidoc.element.errors.Http423Error.Http423Error)
- description and source-code
```javascript
Http423Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http423Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http423Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http423Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http423Error.prototype"></a>[module errors.Http423Error.prototype](#apidoc.module.errors.Http423Error.prototype)

#### <a name="apidoc.element.errors.Http423Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http423Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http423Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http423Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http423Error.prototype.</span>toString ()](#apidoc.element.errors.Http423Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http424Error"></a>[module errors.Http424Error](#apidoc.module.errors.Http424Error)

#### <a name="apidoc.element.errors.Http424Error.Http424Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http424Error (msg, expl, fix)](#apidoc.element.errors.Http424Error.Http424Error)
- description and source-code
```javascript
Http424Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...

For example:
'''js
errors.mapper('RangeError', function(rangeError) {
    return new errors.Http412Error('Invalid range requested');
})
.mapper('ReferenceError', function(refError) {
    return new errors.Http424Error('Bad reference given');
})
.mapper('SyntaxError', function(syntaxError) {
    return new errors.Http400Error('Invalid syntax');
});

// ...
...
```

#### <a name="apidoc.element.errors.Http424Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http424Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http424Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http424Error.prototype"></a>[module errors.Http424Error.prototype](#apidoc.module.errors.Http424Error.prototype)

#### <a name="apidoc.element.errors.Http424Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http424Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http424Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http424Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http424Error.prototype.</span>toString ()](#apidoc.element.errors.Http424Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http425Error"></a>[module errors.Http425Error](#apidoc.module.errors.Http425Error)

#### <a name="apidoc.element.errors.Http425Error.Http425Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http425Error (msg, expl, fix)](#apidoc.element.errors.Http425Error.Http425Error)
- description and source-code
```javascript
Http425Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http425Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http425Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http425Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http425Error.prototype"></a>[module errors.Http425Error.prototype](#apidoc.module.errors.Http425Error.prototype)

#### <a name="apidoc.element.errors.Http425Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http425Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http425Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http425Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http425Error.prototype.</span>toString ()](#apidoc.element.errors.Http425Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http426Error"></a>[module errors.Http426Error](#apidoc.module.errors.Http426Error)

#### <a name="apidoc.element.errors.Http426Error.Http426Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http426Error (msg, expl, fix)](#apidoc.element.errors.Http426Error.Http426Error)
- description and source-code
```javascript
Http426Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http426Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http426Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http426Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http426Error.prototype"></a>[module errors.Http426Error.prototype](#apidoc.module.errors.Http426Error.prototype)

#### <a name="apidoc.element.errors.Http426Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http426Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http426Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http426Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http426Error.prototype.</span>toString ()](#apidoc.element.errors.Http426Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http428Error"></a>[module errors.Http428Error](#apidoc.module.errors.Http428Error)

#### <a name="apidoc.element.errors.Http428Error.Http428Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http428Error (msg, expl, fix)](#apidoc.element.errors.Http428Error.Http428Error)
- description and source-code
```javascript
Http428Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http428Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http428Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http428Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http428Error.prototype"></a>[module errors.Http428Error.prototype](#apidoc.module.errors.Http428Error.prototype)

#### <a name="apidoc.element.errors.Http428Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http428Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http428Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http428Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http428Error.prototype.</span>toString ()](#apidoc.element.errors.Http428Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http429Error"></a>[module errors.Http429Error](#apidoc.module.errors.Http429Error)

#### <a name="apidoc.element.errors.Http429Error.Http429Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http429Error (msg, expl, fix)](#apidoc.element.errors.Http429Error.Http429Error)
- description and source-code
```javascript
Http429Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http429Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http429Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http429Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http429Error.prototype"></a>[module errors.Http429Error.prototype](#apidoc.module.errors.Http429Error.prototype)

#### <a name="apidoc.element.errors.Http429Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http429Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http429Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http429Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http429Error.prototype.</span>toString ()](#apidoc.element.errors.Http429Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http431Error"></a>[module errors.Http431Error](#apidoc.module.errors.Http431Error)

#### <a name="apidoc.element.errors.Http431Error.Http431Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http431Error (msg, expl, fix)](#apidoc.element.errors.Http431Error.Http431Error)
- description and source-code
```javascript
Http431Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http431Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http431Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http431Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http431Error.prototype"></a>[module errors.Http431Error.prototype](#apidoc.module.errors.Http431Error.prototype)

#### <a name="apidoc.element.errors.Http431Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http431Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http431Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http431Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http431Error.prototype.</span>toString ()](#apidoc.element.errors.Http431Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http451Error"></a>[module errors.Http451Error](#apidoc.module.errors.Http451Error)

#### <a name="apidoc.element.errors.Http451Error.Http451Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http451Error (msg, expl, fix)](#apidoc.element.errors.Http451Error.Http451Error)
- description and source-code
```javascript
Http451Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http451Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http451Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http451Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http451Error.prototype"></a>[module errors.Http451Error.prototype](#apidoc.module.errors.Http451Error.prototype)

#### <a name="apidoc.element.errors.Http451Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http451Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http451Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http451Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http451Error.prototype.</span>toString ()](#apidoc.element.errors.Http451Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http500Error"></a>[module errors.Http500Error](#apidoc.module.errors.Http500Error)

#### <a name="apidoc.element.errors.Http500Error.Http500Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http500Error (msg, expl, fix)](#apidoc.element.errors.Http500Error.Http500Error)
- description and source-code
```javascript
Http500Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
...
naming convention 'Http[code]Error'. For example 'Http401Error' and
'Http500Error' which have a code of '401' and '500' respectively.

For example to leverage the HTTP errors:
'''js
throw new errors.Http401Error();
// ...
throw new errors.Http500Error('Something bad happened');
'''

## Connect/Express middleware integration

**Compatibility**
Errors version 0.1.0 only works with Express < 4.0.0.
...
```

#### <a name="apidoc.element.errors.Http500Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http500Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http500Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http500Error.prototype"></a>[module errors.Http500Error.prototype](#apidoc.module.errors.Http500Error.prototype)

#### <a name="apidoc.element.errors.Http500Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http500Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http500Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http500Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http500Error.prototype.</span>toString ()](#apidoc.element.errors.Http500Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http501Error"></a>[module errors.Http501Error](#apidoc.module.errors.Http501Error)

#### <a name="apidoc.element.errors.Http501Error.Http501Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http501Error (msg, expl, fix)](#apidoc.element.errors.Http501Error.Http501Error)
- description and source-code
```javascript
Http501Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http501Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http501Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http501Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http501Error.prototype"></a>[module errors.Http501Error.prototype](#apidoc.module.errors.Http501Error.prototype)

#### <a name="apidoc.element.errors.Http501Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http501Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http501Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http501Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http501Error.prototype.</span>toString ()](#apidoc.element.errors.Http501Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http502Error"></a>[module errors.Http502Error](#apidoc.module.errors.Http502Error)

#### <a name="apidoc.element.errors.Http502Error.Http502Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http502Error (msg, expl, fix)](#apidoc.element.errors.Http502Error.Http502Error)
- description and source-code
```javascript
Http502Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http502Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http502Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http502Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http502Error.prototype"></a>[module errors.Http502Error.prototype](#apidoc.module.errors.Http502Error.prototype)

#### <a name="apidoc.element.errors.Http502Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http502Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http502Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http502Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http502Error.prototype.</span>toString ()](#apidoc.element.errors.Http502Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http503Error"></a>[module errors.Http503Error](#apidoc.module.errors.Http503Error)

#### <a name="apidoc.element.errors.Http503Error.Http503Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http503Error (msg, expl, fix)](#apidoc.element.errors.Http503Error.Http503Error)
- description and source-code
```javascript
Http503Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http503Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http503Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http503Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http503Error.prototype"></a>[module errors.Http503Error.prototype](#apidoc.module.errors.Http503Error.prototype)

#### <a name="apidoc.element.errors.Http503Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http503Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http503Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http503Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http503Error.prototype.</span>toString ()](#apidoc.element.errors.Http503Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http504Error"></a>[module errors.Http504Error](#apidoc.module.errors.Http504Error)

#### <a name="apidoc.element.errors.Http504Error.Http504Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http504Error (msg, expl, fix)](#apidoc.element.errors.Http504Error.Http504Error)
- description and source-code
```javascript
Http504Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http504Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http504Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http504Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http504Error.prototype"></a>[module errors.Http504Error.prototype](#apidoc.module.errors.Http504Error.prototype)

#### <a name="apidoc.element.errors.Http504Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http504Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http504Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http504Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http504Error.prototype.</span>toString ()](#apidoc.element.errors.Http504Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http505Error"></a>[module errors.Http505Error](#apidoc.module.errors.Http505Error)

#### <a name="apidoc.element.errors.Http505Error.Http505Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http505Error (msg, expl, fix)](#apidoc.element.errors.Http505Error.Http505Error)
- description and source-code
```javascript
Http505Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http505Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http505Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http505Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http505Error.prototype"></a>[module errors.Http505Error.prototype](#apidoc.module.errors.Http505Error.prototype)

#### <a name="apidoc.element.errors.Http505Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http505Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http505Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http505Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http505Error.prototype.</span>toString ()](#apidoc.element.errors.Http505Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http506Error"></a>[module errors.Http506Error](#apidoc.module.errors.Http506Error)

#### <a name="apidoc.element.errors.Http506Error.Http506Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http506Error (msg, expl, fix)](#apidoc.element.errors.Http506Error.Http506Error)
- description and source-code
```javascript
Http506Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http506Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http506Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http506Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http506Error.prototype"></a>[module errors.Http506Error.prototype](#apidoc.module.errors.Http506Error.prototype)

#### <a name="apidoc.element.errors.Http506Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http506Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http506Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http506Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http506Error.prototype.</span>toString ()](#apidoc.element.errors.Http506Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http507Error"></a>[module errors.Http507Error](#apidoc.module.errors.Http507Error)

#### <a name="apidoc.element.errors.Http507Error.Http507Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http507Error (msg, expl, fix)](#apidoc.element.errors.Http507Error.Http507Error)
- description and source-code
```javascript
Http507Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http507Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http507Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http507Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http507Error.prototype"></a>[module errors.Http507Error.prototype](#apidoc.module.errors.Http507Error.prototype)

#### <a name="apidoc.element.errors.Http507Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http507Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http507Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http507Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http507Error.prototype.</span>toString ()](#apidoc.element.errors.Http507Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http508Error"></a>[module errors.Http508Error](#apidoc.module.errors.Http508Error)

#### <a name="apidoc.element.errors.Http508Error.Http508Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http508Error (msg, expl, fix)](#apidoc.element.errors.Http508Error.Http508Error)
- description and source-code
```javascript
Http508Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http508Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http508Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http508Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http508Error.prototype"></a>[module errors.Http508Error.prototype](#apidoc.module.errors.Http508Error.prototype)

#### <a name="apidoc.element.errors.Http508Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http508Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http508Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http508Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http508Error.prototype.</span>toString ()](#apidoc.element.errors.Http508Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http509Error"></a>[module errors.Http509Error](#apidoc.module.errors.Http509Error)

#### <a name="apidoc.element.errors.Http509Error.Http509Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http509Error (msg, expl, fix)](#apidoc.element.errors.Http509Error.Http509Error)
- description and source-code
```javascript
Http509Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http509Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http509Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http509Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http509Error.prototype"></a>[module errors.Http509Error.prototype](#apidoc.module.errors.Http509Error.prototype)

#### <a name="apidoc.element.errors.Http509Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http509Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http509Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http509Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http509Error.prototype.</span>toString ()](#apidoc.element.errors.Http509Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http510Error"></a>[module errors.Http510Error](#apidoc.module.errors.Http510Error)

#### <a name="apidoc.element.errors.Http510Error.Http510Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http510Error (msg, expl, fix)](#apidoc.element.errors.Http510Error.Http510Error)
- description and source-code
```javascript
Http510Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http510Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http510Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http510Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http510Error.prototype"></a>[module errors.Http510Error.prototype](#apidoc.module.errors.Http510Error.prototype)

#### <a name="apidoc.element.errors.Http510Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http510Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http510Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http510Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http510Error.prototype.</span>toString ()](#apidoc.element.errors.Http510Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.Http511Error"></a>[module errors.Http511Error](#apidoc.module.errors.Http511Error)

#### <a name="apidoc.element.errors.Http511Error.Http511Error"></a>[function <span class="apidocSignatureSpan">errors.</span>Http511Error (msg, expl, fix)](#apidoc.element.errors.Http511Error.Http511Error)
- description and source-code
```javascript
Http511Error = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.Http511Error.super_"></a>[function <span class="apidocSignatureSpan">errors.Http511Error.</span>super_ (msg, expl, fix)](#apidoc.element.errors.Http511Error.super_)
- description and source-code
```javascript
super_ = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.Http511Error.prototype"></a>[module errors.Http511Error.prototype](#apidoc.module.errors.Http511Error.prototype)

#### <a name="apidoc.element.errors.Http511Error.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.Http511Error.prototype.</span>toJSON ()](#apidoc.element.errors.Http511Error.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.Http511Error.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.Http511Error.prototype.</span>toString ()](#apidoc.element.errors.Http511Error.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.HttpError"></a>[module errors.HttpError](#apidoc.module.errors.HttpError)

#### <a name="apidoc.element.errors.HttpError.HttpError"></a>[function <span class="apidocSignatureSpan">errors.</span>HttpError (msg, expl, fix)](#apidoc.element.errors.HttpError.HttpError)
- description and source-code
```javascript
HttpError = function (msg, expl, fix) {
	var attrs = {};
	if (typeof msg !== null && typeof msg === 'object') {
		attrs = msg;
		msg = attrs['message'] || defaultMessage;
		if (attrs.hasOwnProperty('stack')
				|| attrs.hasOwnProperty('name')
				|| attrs.hasOwnProperty('code')) {
			throw Error("Properties 'stack', 'name' or 'code' " +
					"cannot be overridden");
		}
	}
	attrs['status'] = attrs['status'] || statusCode;
    msg = msg || defaultMessage;
    expl = expl || defaultExplanation;
    fix = fix || defaultResponse;

    parent.call(this, msg);

    // hack around the defineProperty for stack so
    // we can delay stack formatting until access
    // for performance reasons
    Error.captureStackTrace(stack, scope[className]);

<span class="apidocCodeCommentSpan">/**
 * Return the stack tracks for the error.
 *
 * @return {String}
 * @api public
 */
</span>    Object.defineProperty(this, 'stack', {
        configurable: true,
        enumerable: false,
        get: function() {
            if (!formattedStack) {
                formattedStack = stack.stack.replace('[object Object]', 'Error: ' + this.message);
            }
            return formattedStack;
        }
    });

/**
 * Return the explanation for this error.
 *
 * @return {String}
 * @api public
*/

    Object.defineProperty(this, 'explanation', {
        value: attrs['explanation'] || expl,
        configurable: true,
        enumerable: true
    });

/**
 * Return the operator response for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'response', {
        value: attrs['response'] || fix,
        configurable: true,
        enumerable: true
    });

/**
 * Return the error code.
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'code', {
        value: attrs['code'] || errorCode,
        configurable: true,
        enumerable: true
    });

/**
 * HTTP status code of this error.
 *
 * If the instance's 'code' is not a valid
 * HTTP status code it's normalized to 500.s
 *
 * @return {Number}
 * @api public
 */

    Object.defineProperty(this, 'status', {
        value: attrs['status'] || (http.STATUS_CODES[errorCode] ? errorCode : 500),
        configurable: true,
        // normalize for http status code and connect compat
        enumerable: true
    });

/**
 * Name of this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'name', {
        value: className,
        configurable: true,
        enumerable: true
    });

/**
 * Message for this error.
 *
 * @return {String}
 * @api public
 */

    Object.defineProperty(this, 'message', {
        value: attrs['message'] || msg,
        configurable: true,
        enumerable: true
    });

    // expose extra conf attrs as properties
    for (var key in attrs) {
		if (!this.hasOwnProperty(key)) {
			Object.defineProperty(this, key, {
	            value: attrs[key],
	            configurable: true,
	            enumerable: true
	        });
		}
	}

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.HttpError.super_"></a>[function <span class="apidocSignatureSpan">errors.HttpError.</span>super_ ()](#apidoc.element.errors.HttpError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.HttpError.prototype"></a>[module errors.HttpError.prototype](#apidoc.module.errors.HttpError.prototype)

#### <a name="apidoc.element.errors.HttpError.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">errors.HttpError.prototype.</span>toJSON ()](#apidoc.element.errors.HttpError.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
    // TODO externalization
    return useStack
            ? mixin(this, {stack: this.stack}, true)
            : mixin(this, {}, true);
}
```
- example usage
```shell
...
method.

For example:
'''js
errors.stacks(true);
new errors.Http413Error().toString();
// => includes stack trace
new errors.Http413Error().toJSON();
// => includes a 'stack' property
'''

You can also use the 'errors.stacks()' method without arguments to
retrieve the current value of stacks.

This allows you to write code like:
...
```

#### <a name="apidoc.element.errors.HttpError.prototype.toString"></a>[function <span class="apidocSignatureSpan">errors.HttpError.prototype.</span>toString ()](#apidoc.element.errors.HttpError.prototype.toString)
- description and source-code
```javascript
toString = function () {

<span class="apidocCodeCommentSpan">    /*!

    The snippet below would allow us to provide connect errorHandler()
    middleware compatible errors, but is too costly. In a 1000 executions
    of toString() it adds ~25% overhead.

    var e = Error();
    Error.captureStackTrace(e);
    if (~e.stack.indexOf("connect/lib/middleware/errorHandler.js")) {
        return this.message;
    }
    */
</span>
    // TODO externalization
    var msg = util.format("%s: %s\nCode: %s", this.name, this.message, this.code);
    if (this.explanation) {
        msg += "\nExplanation: " + this.explanation;
    }
    if (this.response) {
        msg += "\nResponse: " + this.response;
    }

    function isExtra(key) {
    	return ['name', 'message', 'status', 'code',
    	        'response', 'explanation', 'stack'].indexOf(key) < 0;
    }

    // extra properties
    Object.keys(this).filter(isExtra).forEach(function(key) {
    	msg += util.format("\n%s: %s", key, this[key]);
    }, this);

    if (useStack) {
        msg += "\n" + this.stack;
    }
    return msg;
}
```
- example usage
```shell
...
'''

Create a very barebones error -- you must specify at least the error name:

'''js
// barebones
errors.create({name: 'RuntimeError'});
console.log(new errors.RuntimeError().toString());
'''

produces:
'''
RuntimeError: An unexpected RuntimeError occurred.
Code: 601
'''
...
```



# <a name="apidoc.module.errors.HttpError.super_"></a>[module errors.HttpError.super_](#apidoc.module.errors.HttpError.super_)

#### <a name="apidoc.element.errors.HttpError.super_.super_"></a>[function <span class="apidocSignatureSpan">errors.HttpError.</span>super_ ()](#apidoc.element.errors.HttpError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.HttpError.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">errors.HttpError.super_.</span>captureStackTrace ()](#apidoc.element.errors.HttpError.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.errors.JS_ERRORS"></a>[module errors.JS_ERRORS](#apidoc.module.errors.JS_ERRORS)

#### <a name="apidoc.element.errors.JS_ERRORS.Error"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>Error ()](#apidoc.element.errors.JS_ERRORS.Error)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.JS_ERRORS.EvalError"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>EvalError ()](#apidoc.element.errors.JS_ERRORS.EvalError)
- description and source-code
```javascript
function EvalError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.JS_ERRORS.RangeError"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>RangeError ()](#apidoc.element.errors.JS_ERRORS.RangeError)
- description and source-code
```javascript
function RangeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.JS_ERRORS.ReferenceError"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>ReferenceError ()](#apidoc.element.errors.JS_ERRORS.ReferenceError)
- description and source-code
```javascript
function ReferenceError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.JS_ERRORS.SyntaxError"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>SyntaxError ()](#apidoc.element.errors.JS_ERRORS.SyntaxError)
- description and source-code
```javascript
function SyntaxError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.JS_ERRORS.TypeError"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>TypeError ()](#apidoc.element.errors.JS_ERRORS.TypeError)
- description and source-code
```javascript
function TypeError() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.errors.JS_ERRORS.URIError"></a>[function <span class="apidocSignatureSpan">errors.JS_ERRORS.</span>URIError ()](#apidoc.element.errors.JS_ERRORS.URIError)
- description and source-code
```javascript
function URIError() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
