# react-loopback

A small library to connect [React](https://facebook.github.io/react/)
components to data in a [LoopBack](http://loopback.io) API without the need for
Flux, Redux, etc.

Inspired by Facebook's [Relay](https://facebook.github.io/relay/). The
motivation comes from their website:

> Queries live next to the views that rely on them, so you can easily reason
> about your app.

# Installation

Install using [npm](https://www.npmjs.com/):

```
$ npm install react-loopback
```

Note that this library depends on `fetch` and `Promise` being available globally.
I recommend using the following polyfills:

- [es6-promise](https://www.npmjs.com/package/es6-promise)
- [whatwg-fetch](https://www.npmjs.com/package/whatwg-fetch)

```
$ npm install es6-promise whatwg-fetch
```

Then on code:

```javascript
import {polyfill} from 'es6-promise';
polyfill();
import 'whatwg-fetch';
```

