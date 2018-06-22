![Prettyhtml Banner](/logo.png)

<h2 align="center">Opinionated Web Component HTML formatter</h2>

<p align="center">
  <a href="https://www.npmjs.com/package/prettyhtml">
    <img alt="npm version" src="https://img.shields.io/npm/v/@starptech/prettyhtml.svg?style=flat-square">
  </a>
</p>

- Remove superfluous white-space but still line-wrap as expected.
- Reorder attributes based on how often they occur.
- Special indentation for [`custom elements`](https://developers.google.com/web/fundamentals/web-components/).
- No content manipulation in attributes or tags.

## Packages

* [prettyhtml](/packages/prettyhtml) CLI and API.
* [prettyhtml-formatter](/packages/prettyhtml-formatter) Formater.
* [prettyhtml-hast-to-html](/packages/prettyhtml-hast-to-html) Stringifier.
* [prettyhtml-parse](/packages/prettyhtml-parse) HTML parser and serializer.
* [prettyhtml-rehype-parse](/packages/prettyhtml-rehype-parse) Adapter between HTML parser and rehype.
* [prettyhtml-hast-util-from-parse](/packages/prettyhtml-hast-util-from-parse) Transform Parse5’s AST to HAST.
* [prettyhtml-hastscript](/packages/prettyhtml-hastscript) Hyperscript compatible DSL for creating virtual HAST trees.

## Install

```
$ npm install @starptech/prettyhtml --global
```

## Command Line

```
$ prettyhtml example.md ./**/*.html
```

## Help

```
$ prettyhtml --help
```

## API

```js
const prettyhtml = require('@starptech/prettyhtml')
const result = prettyhtml(`<element></element>`)
```

## TODO

* [ ] Support casesensitive html attributes
* [ ] Fixed tests from packages
* [ ] Agree on ruleset

## Why

Prettier has no support for HTML.


## Acknowledgement

Big thanks to the creators of the excellent [rehype](https://github.com/rehypejs/rehype) and [unified](https://github.com/unifiedjs/unified) ecosystem.
