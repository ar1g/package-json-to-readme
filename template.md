# {{name}} {{#travis_url}}[![Build Status]({{travis_url}}.png?branch=master)]({{travis_url}}){{/travis_url}}

{{description}}

{{#usage}}
## Usage

```{{language}}
{{{content}}}
```
{{/usage}}

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
