# @lfgroup/codegen-js-converter

Micro (1.8 kB) `graphql-codegen` plugin, that converts enums from provided GraphQL server schema to a file with JS objects.

### Example

Taking following gql schema, this plugin would generate code below. It is convinient to use generated result in a pre-compiled enviroment such as `next.config.js`

```gql
enum WowRole {
  Healer
  Damage
  Tank
}
```

```js
const WowRole = {
  Healer: 'Healer',
  Damage: 'Damage',
  Tank: 'Tank'
};
```

### Usage

In your YAML config file add a new generated file with this plugin as stated:

```yml
generates:
  src/generated/types.js:
    plugins:
      - '@lfgroup/codegen-js-converter'
```
