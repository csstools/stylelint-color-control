# Stylelint Color Control [<img src="https://jonathantneal.github.io/stylelint-logo.svg" alt="stylelint" width="90" height="90" align="right">][stylelint]

[![NPM Version][npm-img]][npm-url]
[![Build Status][cli-img]][cli-url]
[![Support Chat][git-img]][git-url]

[Stylelint Color Control] is a [stylelint] rule to control color usage in CSS.

## Usage

Add [stylelint] and [Stylelint Color Control] to your project.

```bash
npm install stylelint stylelint-color-control --save-dev
```

Add [Stylelint Color Control] to your [stylelint configuration].

```js
{
  "plugins": [
    "stylelint-color-control"
  ],
  "rules": {
    "csstools/stylelint-color-control": "always" || "never" || "ignore"
  }
}
```

## Options

### always

If the first option is `"always"` or `true`, then [Stylelint Color Control] requires all
nodes to be linted, and the following patterns are _not_ considered violations:

```pcss
.example {}
```

While the following patterns are considered violations:

```pcss
.example {}
```

### never

If the first option is `"never"` or `false`, then [Stylelint Color Control] requires all 
nodes to be linted, and the following patterns are _not_ considered
violations:

```pcss
.example {}
```

While the following patterns are considered violations:

```pcss
.example {}
```

### ignore

If the first option is `"ignore"` or `null`, then [Stylelint Color Control] does nothing.

[cli-img]: https://img.shields.io/travis/csstools/stylelint-color-control.svg
[cli-url]: https://travis-ci.org/csstools/stylelint-color-control
[git-img]: https://img.shields.io/badge/support-chat-blue.svg
[git-url]: https://gitter.im/stylelint/stylelint
[npm-img]: https://img.shields.io/npm/v/stylelint-color-control.svg
[npm-url]: https://www.npmjs.com/package/stylelint-color-control

[stylelint]: https://github.com/stylelint/stylelint
[stylelint configuration]: https://github.com/stylelint/stylelint/blob/master/docs/user-guide/configuration.md#readme
[Stylelint Color Control]: https://github.com/csstools/stylelint-color-control
