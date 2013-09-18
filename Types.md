# Generic Types

- Numbers
- Strings
- Booleans
- Functions
- Objects

## Numbers

- Integers - `5`, `42`, `5322241`
- Floats - `0.5`, `12.098`
- `Math.*` - contains math functions and constants. Examples:
    - `Math.max()` / `Math.min()`
    - `Math.floor()` /  `Math.ceil()`
    - `Math.PI`
- `parseInt()`, `parseFloat()`, and the `+` operator
- Special Cases - `Infinity`, `-Infinity`, and `NaN`

## Strings

Any sequence of characters. String literals can be encapsulated in single- (`'`) and double-quotes (`"`).

    "hello".length // 5
    "hello".charAt(0) // h
    "hello, world".replace("hello", "goodbye") // goodbye, world
    "hello".toUpperCase() // HELLO

## Booleans

`true` and `false`. Useful in control structures when deciding whether to execute an operation.

`false`, `0`, the empty string (`""`), `NaN`, `null`, and `undefined` are all interpreted as `false`. All other values are interpreted as `true`.

    false == false // true
    0 == false // true
    '0' == false // false. notice the string
