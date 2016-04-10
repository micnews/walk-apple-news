# walk-apple-news [![Build Status](https://travis-ci.org/micnews/walk-apple-news.png?branch=master)](https://travis-ci.org/micnews/walk-apple-news)

Walk &amp; do inline transformations of an apple news feed

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
npm install walk-apple-news --save
```

## Usage

```js
import walk from './';

const appleNewsFormat = {
  components: [{
    role: 'container',
    components: [{
      role: 'container',
      components: [{
        role: 'photo',
        URL: 'bundle://image-1'
      }]
    }]
  }]
};

walk(appleNewsFormat, function (component) {
  console.log('component', component);
});

```

## Tests

```sh
npm install
npm test
```

## Dependencies

None

## Dev Dependencies

- [ava](https://github.com/sindresorhus/ava): Futuristic test runner 🚀
- [babel-cli](https://github.com/babel/babel/tree/master/packages): Babel command line.
- [babel-core](https://github.com/babel/babel/tree/master/packages): Babel compiler core.
- [babel-preset-es2015](https://github.com/babel/babel/tree/master/packages): Babel preset for all es2015 plugins.
- [semistandard](https://github.com/Flet/semistandard): All the goodness of `feross/standard` with semicolons sprinkled on top.
- [snazzy](https://github.com/feross/snazzy): Format JavaScript Standard Style as Stylish (i.e. snazzy) output


## License

MIT

_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_