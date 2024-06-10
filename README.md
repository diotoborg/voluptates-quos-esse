# @diotoborg/voluptates-quos-esse <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Map? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isMap = require('@diotoborg/voluptates-quos-esse');
assert(!isMap(function () {}));
assert(!isMap(null));
assert(!isMap(function* () { yield 42; return Infinity; });
assert(!isMap(Symbol('foo')));
assert(!isMap(1n));
assert(!isMap(Object(1n)));

assert(!isMap(new Set()));
assert(!isMap(new WeakSet()));
assert(!isMap(new WeakMap()));

assert(isMap(new Map()));

class MyMap extends Map {}
assert(isMap(new MyMap()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@diotoborg/voluptates-quos-esse
[npm-version-svg]: https://versionbadg.es/inspect-js/@diotoborg/voluptates-quos-esse.svg
[deps-svg]: https://david-dm.org/inspect-js/@diotoborg/voluptates-quos-esse.svg
[deps-url]: https://david-dm.org/inspect-js/@diotoborg/voluptates-quos-esse
[dev-deps-svg]: https://david-dm.org/inspect-js/@diotoborg/voluptates-quos-esse/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@diotoborg/voluptates-quos-esse#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@diotoborg/voluptates-quos-esse.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@diotoborg/voluptates-quos-esse.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@diotoborg/voluptates-quos-esse.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@diotoborg/voluptates-quos-esse
[codecov-image]: https://codecov.io/gh/inspect-js/@diotoborg/voluptates-quos-esse/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@diotoborg/voluptates-quos-esse/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@diotoborg/voluptates-quos-esse
[actions-url]: https://github.com/diotoborg/voluptates-quos-esse/actions
