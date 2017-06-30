# babel-plugin-transform-vue-template

[![NPM version](https://img.shields.io/npm/v/babel-plugin-transform-vue-template.svg?style=flat)](https://npmjs.com/package/babel-plugin-transform-vue-template) [![NPM downloads](https://img.shields.io/npm/dm/babel-plugin-transform-vue-template.svg?style=flat)](https://npmjs.com/package/babel-plugin-transform-vue-template) [![CircleCI](https://circleci.com/gh/egoist/babel-plugin-transform-vue-template/tree/master.svg?style=shield)](https://circleci.com/gh/egoist/babel-plugin-transform-vue-template/tree/master)  [![donate](https://img.shields.io/badge/$-donate-ff69b4.svg?maxAge=2592000&style=flat)](https://github.com/egoist/donate)

An alternative way to use Vue `template` and compile it at build time.

## Install

```bash
yarn add vue-template-compiler babel-plugin-transform-vue-template --dev
# vue-template-compiler is required as peer dependency
```

## Usage

With `.babelrc`:

```js
{
  "plugins": ["transform-vue-template"]
}
```

Then you can write `template` in your `render` function:

```js
import pokemon from 'pokemon'

export default {
  render() {
    return `<div>
      <h1>Hello,  I'm a random pokemon: ${pokemon.random()}</h1>
      <button @click="whatever">Click me!</button>
    </div>`
  },
  methods: {
    whatever() {
      // do whatever
    }
  }
}
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D


## Author

**babel-plugin-transform-vue-template** © [egoist](https://github.com/egoist), Released under the [MIT](./LICENSE) License.<br>
Authored and maintained by egoist with help from contributors ([list](https://github.com/egoist/babel-plugin-transform-vue-template/contributors)).

> [egoistian.com](https://egoistian.com) · GitHub [@egoist](https://github.com/egoist) · Twitter [@rem_rin_rin](https://twitter.com/rem_rin_rin)