# Getting Started
  
## Install

**Via NPM:** (preferred)

_Latest stable release:_

- `npm install --save cornerstone-tools`

_Pre-release, unstable, mostly for contributors:_

- `npm install --save cornerstone-tools@next`

## Usage

See the [live examples](https://rawgithub.com/cornerstonejs/cornerstoneTools/master/examples/index.html) and [wiki](https://github.com/cornerstonejs/cornerstoneTools/wiki) for documentation (Soon to be replaced by [tools.cornerstonejs.org](http://tools.cornerstonejs.org/)) on how to use this library

**A common setup when using modules:**

```javascript
import Hammer from "hammerjs";
import * as cornerstone from "cornerstone-core";
import * as cornerstoneTools from "cornerstone-tools";

cornerstoneTools.external.cornerstone = cornerstone;
cornerstoneTools.external.Hammer = Hammer;
```

# Contributing

**How To Contribute:**

1.  Fork this repository
2.  Clone the forked repository
3.  Before committing code, create a branch-per-feature, or branch-per-bug
4.  Create pull requests against `cornerstonejs/cornerstoneTools/master`

# Build System

This project uses webpack to build the software.

**Requirements:**

- [NodeJs](http://nodejs.org).

**Common Tasks:**

Update dependencies (after each pull):

> npm install

Running the build:

> npm start

Automatically running the build and unit tests after each source change:

> npm run watch

[license-image]: http://img.shields.io/badge/license-MIT-blue.svg?style=flat
[license-url]: LICENSE
[npm-url]: https://npmjs.org/package/cornerstone-tools
[npm-version-image]: http://img.shields.io/npm/v/cornerstone-tools.svg?style=flat
[npm-downloads-image]: http://img.shields.io/npm/dm/cornerstone-tools.svg?style=flat
[travis-url]: http://travis-ci.org/cornerstonejs/cornerstoneTools
[travis-image]: https://travis-ci.org/cornerstonejs/cornerstoneTools.svg?branch=master
[coverage-url]: https://coveralls.io/github/cornerstonejs/cornerstoneTools?branch=master
[coverage-image]: https://coveralls.io/repos/github/cornerstonejs/cornerstoneTools/badge.svg?branch=master
