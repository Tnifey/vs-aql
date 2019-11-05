`vs-aql` is prototype of language extension for `aql` from ArangoDB with basic support of `aql` tag, `.aql` files syntax highlight and snippets

should work with .aql, .js, .jsx, .ts, .tsx files

## Features

- basic support for syntax hightlight
- snippets for functions
- works with ArangoJS `aql` tagged template literal

## Release Notes

### 0.0.2

👍

- template literal without aql tag works with comment `//aql`

```ts
aql`
for user in Users
  limit 1
...
```

```ts
notAnAqlTag`//aql    <-- note for comment
for user in Users
  limit 1
...
```

- ternery operator
- basic function highlight
- `@variable` highlight

👎

- `aql` tag not working properly - use comment `//aql` instead
- drop `.vue` support

### 0.0.1

👍

Basic support for basic things.

- basic syntax hightlight
- snippets
- `aql` tag support
- `aql` tag supports inline \${javascript + expressions}

👎

- `aql.literal()` won't work properly
- regular expressions won't syntax highlight

## License

MIT
