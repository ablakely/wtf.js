# wtf.js
wtf.js is a [JSFuck](https://en.wikipedia.org/wiki/JSFuck) compiler written in C.

## Building

    make

## Usage

    ./wtf in.js out.js

## How does this work?
wtf.js uses type coercion to produce working, yet unreadable javascript.

I recommed checking out [this video by Low Level Javascript](https://www.youtube.com/watch?v=sRWE5tnaxlI) if you're interested in learning more.

## Runtimes
### Node.js
To use `require` you must define it, like so:

    const require = new Function("var require = global.require || global.process.mainModule.constructor._load; return require")();

## Support
Support for wtf.js is available on [IRC](https://webchat.ephasic.org/?join=ephasic)
