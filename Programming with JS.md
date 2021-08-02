# [Programming with JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

JavaScript has the following types of operators. 
- Assignment operators
- Comparison operators
-	Arithmetic operators
-	Bitwise operators
-	Logical operators
-	String operators
-	Conditional (ternary) operator
- Comma operator
-	Unary operators
-	Relational operators

JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator. 
A binary operator requires two operands, one before the operator and one after the operator:
operand1 operator operand2

For example, 3+4 or x*y.
A unary operator requires a single operand, either before or after the operator:
operator operand
or
operand operator



## Assignment operators

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = y assigns the value of y to x.
There are also compound assignment operators that are shorthand for the operations listed in the following table:

Return value and chaining
- Like most expressions, assignments like x = y have a return value. It can be retrieved by e.g. assigning the expression or logging it:
const z = (x = y); // Or equivalently: const z = x = y;

- console.log(z); // Log the return value of the assignment x = y.
console.log(x = y); // Or log the return value directly.
The return value matches the expression to the right of the = sign in the “Meaning” column of the table above. 
That means that (x = y) returns y, (x += y) returns the resulting sum x + y, (x * * = y) returns the resulting power x ** y, and so on.

- In the case of logical assignments, (x &&= y), (x ||= y), and (x ??= y), the return value is that of the logical operation without the assignment, so x && y, x || y, and x ?? y, respectively.
Note that the return values are always based on the operands’ values before the operation.
When chaining these expressions, each assignment is evaluated right-to-left. Consider these examples:
•	w = z = x = y is equivalent to w = (z = (x = y)) or x = y; z = y; w = y
•	z += x *= y is equivalent to z += (x *= y) or tmp = x * y; x *= y; z += tmp (except without the tmp).

## Destructuring
For more complex assignments, the destructuring assignment syntax is a JavaScript expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.
var foo = ['one', 'two', 'three'];

// without destructuring
var one   = foo[0];
var two   = foo[1];
var three = foo[2];

// with destructuring
var [one, two, three] = foo;

- Comparison operators
A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. These operators do not attempt to convert the operands to compatible types before checking equality. The following table describes the comparison operators in terms of this sample code:
var var1 = 3;
var var2 = 4;
Note: => is not an operator, but the notation for Arrow functions.

- Arithmetic operators
An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value. The standard arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). These operators work as they do in most other programming languages when used with floating point numbers (in particular, note that division by zero produces Infinity). For example:
1 / 2; // 0.5
1 / 2 == 1.0 / 2.0; // this is true
Bitwise operators
A bitwise operator treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers. For example, the decimal number nine has a binary representation of 1001. Bitwise operators perform their operations on such binary representations, but they return standard JavaScript numerical values.


## Bitwise logical operators
Conceptually, the bitwise logical operators work as follows:
    - The operands are converted to thirty-two-bit integers and expressed by a series of bits (zeros and ones). Numbers with more than 32 bits get their most significant bits discarded. For example, the following integer with more than 32 bits will be converted to a 32 bit integer:
    - Before: 1110 0110 1111 1010 0000 0000 0000 0110 0000 0000 0001
    - After:               1010 0000 0000 0000 0110 0000 0000 0001
    - Each bit in the first operand is paired with the corresponding bit in the second operand: first bit to first bit, second bit to second bit, and so on.
    - The operator is applied to each pair of bits, and the result is constructed bitwise.
 
- Bitwise shift operators

The bitwise shift operators take two operands: the first is a quantity to be shifted, and the second specifies the number of bit positions by which the first operand is to be shifted. The direction of the shift operation is controlled by the operator used.
Shift operators convert their operands to thirty-two-bit integers and return a result of either type Number or BigInt: specifically, if the type of the left operand is BigInt, they return BigInt; otherwise, they return Number.

- Logical operators

Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. 

## Functions

Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.
See also the exhaustive reference chapter about JavaScript functions to get to know the details.
Defining functions

- Function declarations
A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:
  -	The name of the function.
  - A list of parameters to the function, enclosed in parentheses and separated by commas.
  - The JavaScript statements that define the function, enclosed in curly brackets, {...}.

- Control flow
The control flow is the order in which the computer executes statements in a script.
Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 
For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:
if (field==empty) {
    promptUser();
} else {
    submitForm();
}

A typical script in JavaScript or PHP (and the like) includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur.
For example, the above excerpt might be inside a function that runs when the user clicks the Submit button for the form. The function could also include a loop, which iterates through all of the fields in the form, checking each one in turn. Looking back at the code in the if and else sections, the lines promptUser and submitForm could also be calls to other functions in the script. As you can see, control structures can dictate complex flows of processing even with only a few lines of code.
Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.


