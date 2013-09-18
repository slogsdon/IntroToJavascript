# Intro To Javascript

A primer into programming in Javascript. This assumes you know nothing, and that's ok.

#### Resources

- [Mozilla Developer Network](https://developer.mozilla.org/en-US/) - covers HTML, CSS, Javascript, Web APIs, etc. Also contains tutorials, awesome explanations, and demos.
- [StackOverflow](http://stackoverflow.com/) - question/answer style website. The higher the score of an answer, the more it is accepted as correct and/or best practice, but don't rule out other answers.

#### Tools of the Trade

- Your trusty text editor. I like [SublimeText](http://www.sublimetext.com/), but use what makes you comfortable.
- Any browser worth its weight. Chrome is awesome for development, but if you use something else, make sure your chosen browser has awesome developer tools as they will help you in the future

#### Respected Developers

- [Douglas Crockford](http://www.crockford.com/) - claim to fame: Javascript best practices

    ![](http://www.crockford.com/goodparts.gif)

- [John Resig](http://ejohn.org/) - claim to fame: jQuery
- [Paul Irish](http://www.paulirish.com/) - claim to fame: Modernizr, HTML5 Boilerplate

## Let's Get to It

We're going to be following [A re-introduction to JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript) on MDN. While it's aimed at devs who already know Javascript, it describes everything you need to know and the reasons for doing things the right way.

### Generic Types

- Numbers
- Strings
- Booleans
- Functions
- Objects

#### Numbers

- Integers - `5`, `42`, `5322241`
- Floats - `0.5`, `12.098`
- `Math.*` - contains math functions and constants. Examples:
    - `Math.max()` / `Math.min()`
    - `Math.floor()` /  `Math.ceil()`
    - `Math.PI`
- `parseInt()`, `parseFloat()`, and the `+` operator
- Special Cases - `Infinity`, `-Infinity`, and `NaN`

#### Strings

Any sequence of characters. String literals can be encapsulated in single- (`'`) and double-quotes (`"`).

    "hello".length // 5
    "hello".charAt(0) // h
    "hello, world".replace("hello", "goodbye") // goodbye, world
    "hello".toUpperCase() // HELLO

#### Booleans

`true` and `false`. Useful in control structures when deciding whether to execute an operation.

`false`, `0`, the empty string (`""`), `NaN`, `null`, and `undefined` are all interpreted as `false`. All other values are interpreted as `true`.

    false == false // true
    0 == false // true
    '0' == false // false. notice the string

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

`==` and `!=` type cast where `===` and `!==` do not.

    1 == true // true
    1 === true // false
