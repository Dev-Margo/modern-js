# Javascript Fundementals
## Variables:
- "let" to declare a variable.
- e.g `"x = 'Hello';`
- var is the older form of let with some differences
- repeated declarations are illegal: 
- SyntaxError: 'message' has already been declared
        
### Naming:
- Names can only have letters, digits, or $ and _
- Use camel case
- cant start with digits
- cant have hyphens in variable Names
- case matters 
- use strict makes declarations without let illegal (i.e. python)
        
### Constants use "const"
+ consts cant be reassigned

## Data Types:
- Javascript is dynamically typed - a variable can contain any datatype

### Number: 
- Contains both ints and floats  
- Also contains Infinity, -Infinity, and NaN  
- Any operations on a NaN value return NaN  
- Math is "Safe" in Javascript, an error will not stop the script  
### BigInt:  
- values larger than (253-1) (that’s 9007199254740991), or less than -(253-1) for negatives.

### String:
- surrounded by quotes "", '', or ``  
- Backticks are extended functionality quotes  
- They let you embed things in strings (like format strings)  
```
// embed a variable  
alert( `Hello, ${name}!` ); // Hello, John!  
```
- No Char type

### Boolean:
- true and false

### null:
- null pointer

### undefined:
- value not defined
        
### objects and symbols:
- mentioned later
        
### typeof operator:
- returns the type of the argument

## Interactions: alert, prompt, confirm
alert:  
- modal, steals focus from the windows

prompt:  
- shows a modal window with a message, an input field, and the OK and cancel button
- takes two args:  
```
result = prompt(title, [default]);
//square brackets mean the argument is optional 
```
        
confirm:  
- shows a modal window with a question and two buttons, ok and cancel
- returns true if OK, false otherwise  
`let isBoss = confirm("Are you the boss?");`
            
## Type Conversions
> Most of the time operators and functions automatically convert to the values given to them

### String Conversion
> Sting(value) for explicit conversion
let value = true;  
```
alert(typeof value); // boolean  
value = String(value); // now value is a string "true"  
alert(typeof value); // string  
```

### Numeric Conversion
> We can user Number(value) function to convert a value to a number

### Boolean Conversion
> Boolean(value) for explicit conversion  
> Conversion rules:
>   Values that are intuitively “empty”, like 0, an empty string, null, undefined, and NaN, become false.  
>   Other values become true.  

## Basic operators, math
### math operators
The following math operations are supported:  
- addition +
- subtraction -
- multiplication *
- division /
- remainder %
- exponentiation **

### String concatenation with + operator
- let s = 'my' + 'string';

### Numeric conversion, unary +
- The unary plus is pplies to a single value that is non numberic will convert that value to a number  
- e.g. it is the same as calling Number(x)

### Operator precedence
- unary first
- then binary

### Assignment
- calculations are done first then assignment is run
### Chained assignments
- evaluate from left to right
- `a = b = c = 2+2;`
- is the same as 
```
c = 2+2;
b = c;
a = c;
```

### Increment and decrement
- ++ and --
- prefix form:
```
let counter = 1;  
let a = ++counter;  
alert(a); //returns 2  
//*increment and return*
```
- postfix form
```
let counter = 1;  
let a = counter++;  
alert(a); //returns 1
alert(counter) //returns 2  
*increment but do NOT return value*
```
### comma
> The comma operator , is one of the rarest and most unusual operators. Sometimes, it’s used to write shorter 
> code, so we need to know it in order to understand what’s going on.
> The comma operator allows us to evaluate several expressions, dividing them with a comma ,. Each of them is  > evaluated but only the result of the last one is returned.  
> ex:  `for (a = 1, b = 3, c = a * b; a < 10; a++) {};`

### bitwise 
- supported as usual see references 

## Comparisons
Javascript comparisons: 
- Greater lesser: ` > < >= <= `  
- Equals ` == ` (equality test)  
- Not Equals ` != `  
- Returns bool

### Strong Comparisons
- Strings are compared letter by letter 
 