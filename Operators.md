### Operators

Boolean operators help test `Boolean` (`true` and `false`) values.

- `&&` - And. Both sides must be true
    - `true && true // true`
    - `true && false // false`
    - `false && false // false`
- `||` - Or. One side must be true. Once a `true` is evaluated, remaining expressions are ignored
    - `true || true // true`
    - `false || true // true`
    - `false || false // false`
- `!` - Not. Inverts an expession's boolean value
    - `!false // true`
    - `!true // false`

Numeric operators

- `+` - addition and string concatenation
    - `5 + 5 // 10`
    - `'hello' + 'world' // 'helloworld'`
    - Watch out! Funny things can happen when applying `+` to numeric and string types at the same time.
- `-` - subtraction
- `*` - multiplication
- `/` - division
    - Integer division - `5 / 2 // 2`
    - Floating point division - `5.0 / 2 // 2.5` 
- `%` - modulus aka the remainder operator
    - Integer division - `5 % 2 // 1`
        - `mod 2` is a great way to test if an `int` is even or odd.
    - Floating point division - `3.5 % 2 // 1.5`
        - Other languages don't offer this and restrict modulus to integers

Comparison operators work on strings and numbers.

- `==` and `===` - equality
- `!=` and `!==` - inequality
- `>` and `>=` - greater than, greater than or equal to
- `<` and `<=` - less than, less than or equal to
