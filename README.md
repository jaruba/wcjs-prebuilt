# <img alt="WebChimera.js Prebuilt" src="https://raw.githubusercontent.com/jaruba/wcjs-logos/master/logos/small/wcjs-prebuilt.png">

![badge](https://nodei.co/npm/wcjs-prebuilt.png?downloads=true)

Install [WebChimera.js](http://github.com/RSATom/WebChimera.js) prebuilt binaries **for Electron** using npm. This module allows you to set-up **WebChimera.js + embedded VLC** without compilation / additional steps.

WebChimera.js is a node.js binding to libvlc. You can use it to play video using a JS raw array buffer drawn via WebGL.


## Installation

```
npm install wcjs-prebuilt
```

You can install the module for another platform than the one you're running - for example if you want to package your application for another OS. To do that, use the ``WCJS_PLATFORM``, ``WCJS_ARCH`` environment variables.
You can also tweak WebChimera.js version through ``WCJS_VERSION``.

For example, to install for Windows under any OS, use
```
WCJS_PLATFORM=win32 WCJS_ARCH=ia32 npm install wcjs-prebuilt
```

Currently supported runtimes are:
* ``electron`` / ``electron44`` - Electron 0.29.x, based on chromium 44
* ``electron45`` - electron 0.31.x, based on chromium 45
* ``nwjs`` - latest NW.js

## Programmatic usage
```javascript
var wcjs = require("wcjs-prebuilt");
// wcjs is WebChimera.js
```

## Used in (ordered by date of adoption)
* [Stremio](www.strem.io) - since version 2.0
* [Powder Player](http://powder.media) - since version 0.90
* [Popcorn Time](https://popcorntime.io) - not yet released with WebChimera.js, in progress


(please PR other use cases)
