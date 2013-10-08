# Control Structures

## `if`

Remember those boolean expressions? `if` uses those to decide whether or not to execute a block of code.

    var num = 5;
    if (num == 5) {
        // do something fun!
    }
    
`else` lets us define code to be executed when the boolean expression is `false`.

    var num = 5;
    if (num == 4) {
        // this doesn't happen
    } else {
        // do something fun!
    }
    
We can even blend `else` with another `if` to test for another case.

    var num = 5;
    if (num == 4) {
        // not going to happen
    } else if (num ==5) {
        // do something fun!
    } else {
        // if all else fails. get it? all ELSE fails
    }
    
### Ternary operator, a.k.a. the `if` shorthand

For simple if statements, the ternary operator can save you some keystrokes and can help clean up your code. 

    var num = 5;
    var myString = (num == 5 ? 'this number is five' : 'this number is not five'); // all three parts are needed!

Watch out! This shouldn't be used for complicated `if` structures

### Short-circuit Logic 

`&&` and `||` allow for conditionally calling a second operand based on the first. Testing for `null`/`undefined` values is the most common reason for doing this.

    // assignment
    var obj = obj || {};
    // execution
    var name = obj && obj.getName();
    
Those two statements can be rewritten as full `if` statements

    // assignment
    var obj;
    if (!obj) {
        obj = {}
    }
    // execution
    var name;
    if (obj) {
        name = obj.getName();
    }

Don't do that though. Writing `if` statements like that can introduce scope problems. 
