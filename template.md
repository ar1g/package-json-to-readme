# {{name}} {{#travis_url}}[![Build Status]({{travis_url}}.png?branch=master)]({{travis_url}}){{/travis_url}}

{{description}}

{{^private}}
## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
{{#preferGlobal}}
npm install {{name}} --global
{{/preferGlobal}}
{{^preferGlobal}}
npm install {{name}} --save
{{/preferGlobal}}
```
{{/private}}

{{#usage}}
## Usage

```{{language}}
{{{content}}}
```
{{/usage}}

{{#scripts.test}}
## Tests

```sh
npm install
npm test
```
{{/scripts.test}}
{{#testOutput}}
```
{{{testOutput}}}
```
{{/testOutput}}

## Scripts

{{#scriptList}}
{{scriptname}}
```sh
{{{scriptcode}}}
```
{{/scriptList}}

## Dependencies

{{#depDetails}}
- [{{name}}]({{repository.url}}): {{description}}
{{/depDetails}}
{{^depDetails}}
None
{{/depDetails}}

## Dev Dependencies

{{#devDepDetails}}
- [{{name}}]({{repository.url}}): {{description}}
{{/devDepDetails}}

{{^devDepDetails}}
None
{{/devDepDetails}}

{{#license}}
## License

{{license}}
{{/license}}

{{#footer}}
_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_
{{/footer}}
