# Javascript Fundementals

## Variables:
> "let" to declare a variable.
+ e.g "x = 'Hello';

> var is the older form of let with some differences

> repeated declarations are illegal: 
+ SyntaxError: 'message' has already been declared
        
### Naming:
+ Names can only have letters, digits, or $ and _
+ Use camel case
+ cant start with digits
+ cant have hyphens in variable Names
+ case matters 
+ use strict makes declarations without let illegal (i.e. python)
        
### Constants use "const"
+ consts cant be reassigned

## Data Types:
> Javascript is dynamically typed - a variable can contain any datatype

        Number: 
            contains both ints and floats
            Also contains Infinity, -Infinity, and NaN 
            Any operations on a NaN value return NaN
            Math is "Safe" in Javascript, an error will not stop the script
        
        BigInt:
            values larger than (253-1) (that’s 9007199254740991), or less than -(253-1) for negatives.

        String:
            surrounded by quotes "", '', or ``
            Backticks are extended functionality quotes
                They let you embed things in strings (like format strings)
                // embed a variable
                alert( `Hello, ${name}!` ); // Hello, John!

        No Char type

        Boolean:
            true and false

        null:
            null pointer

        undefined:
            value not defined
        
        objects and symbols:
            mentioned later
        
        typeof operator:
            returns the type of the argument

## Interactions: alert, prompt, confirm
        alert:
            modal, steals focus from the windows

        prompt:
            shows a modal window with a message, an input field, and the OK and cancel button
            takes two args:
                result = prompt(title, [default]);
                //square brackets mean the argument is optional
        
        confirm:
            shows a modal window with a question and two buttons, ok and cancel
                returns true if OK, false otherwise
                let isBoss = confirm("Are you the boss?");
            

