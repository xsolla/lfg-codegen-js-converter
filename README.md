# @lfgroup/codegen-js-converter

Micro (1.8 kB) `graphql-codegen` plugin, that converts enums from client schema to a JS objects.

### Usage

In your YAML config file add a new generated file with this plugin as stated:

```yml
generates:
  src/generated/types.js:
    plugins:
      - @lfgroup/codegen-js-converter
```
