# JavaScript

---

### What is JavaScript?

JavaScript is a high-level scripting or programming language primarily used for building dynamic and interactive web pages.

"Tired of static web pages? Let JavaScript breathe life into your projects!"

### Brief History and Evolution

Yes!, JavaScript is not derived from Java ! , JavaScript was first developed by Brendan Eich at Netscape Communications Corporation. Originally named Mocha, it was later renamed to LiveScript before settling on JavaScript. Over the years, JavaScript has undergone significant evolution and is now widely used not only in web development but also in server-side and mobile app development.

### Role of JavaScript in web development

JavaScript plays a crucial role in web development by allowing developers to add interactivity, dynamic content, and behavior to web pages. It is used to handle user interactions, manipulate the DOM (Document Object Model), make asynchronous requests to servers, and much more.

"Feeling overwhelmed by terms like DOM and Asynchronous? Don't worry, you'll become familiar with them soon enough!"

### Setting Up Your Development Environment

To write and run JavaScript code, you'll need a code editor. Here are a few popular options:

- **Visual Studio Code**: A powerful and customizable code editor developed by Microsoft.
- **Sublime Text**: A lightweight and fast code editor with a rich ecosystem of plugins.
- **Atom**: A hackable text editor built by GitHub.

### Running JavaScript in a Browser Console

All modern web browsers come with a built-in JavaScript console where you can execute `JavaScript` code directly within the browser. Here's how to access it:

1. Open your web browser.
2. Right-click on any webpage and select **Inspect** or press `Ctrl+Shift+I` (Windows/Linux) or `Cmd+Option+I` (Mac) to open the Developer Tools.
3. Navigate to the **Console** tab.
4. You can now type and execute JavaScript code directly in the console.

### Your First Code !

```javascript
console.log("Hello world!");
```

This simple line of code will print "Hello World" in your browser's console. Go ahead, try it out!

Do you want to personalize this message?

```javascript
let a = "Alice";
console.log(`Hello ${a}!`);
```

Try changing the value of name to your own name!

### Explanation:

- The backticks (\`) are used to create template literals in JavaScript.
- Inside a template literal, you can embed expressions using `${}` syntax.
- When JavaScript encounters `${}`, it evaluates the expression inside the curly braces and includes the result in the string.

## JavaScript Variables and Data Types

Variables are used to store data values in JavaScript. JavaScript supports various data types, each serving different purposes. Majorly data types are :

- **Numbers**
- **Strings**
- **Booleans**
- **Arrays**
- **Objects**

Let's explore the different data types and their key points:

### Numbers

JavaScript represents numbers using the number data type. Numbers can be integers , floating-point numbers or negative numbers.

```javascript
let age = 25;
let pi = 3.14;
```

### Strings

Strings are sequences of characters enclosed within single quotes ('') or double quotes (""). Strings are immutable(cannot be modified once declared).

```javascript
let name = "Alice";
let message = "Hello, world!";
```

### Booleans

Booleans represent logical values: true or false. They are commonly used in conditional statements and logical expressions.

```javascript
let isStudent = true;
let isValid = false;
```

### Arrays

Arrays are ordered collections of values, each identified by an index. They can contain elements of different data types.

```javascript
let numbers = [1, 2, 3, false, "yellow"];
let colors = ["red", "green", "blue", true];
```

### Objects

Objects are collections of key-value pairs, where keys are strings and values can be any data type.

```javascript
let person = { name: "John", age: 30 };
let book = { title: "JavaScript Basics", pages: 100 };
```

### Creation of Objects

You can create objects in JavaScript using either object literal notation `{}` or the `Object()` constructor.

```javascript
// Using object literal notation
let person = {
  name: "John",
  age: 30,
  city: "New York",
};

// Using Object() constructor
let car = new Object();
car.make = "Toyota";
car.model = "Corolla";
car.year = 2020;
```

### Accessing Object Properties

You can access the values of object properties in JavaScript using dot notation or bracket notation.

- **Dot Notation**

In dot notation, you use a dot (`.`) followed by the property name to access the value of the property.

```javascript
console.log(person.name); // Output: John
```

- **Bracket Notation**

In bracket notation, you use square brackets `([])` with the property name enclosed in quotes to access the value of the property.

```javascript
console.log(book["title"]); // Output: JavaScript Basics
```

### Adding and Deleting Object Properties

You can add new properties to an object or delete existing ones using the assignment operator `(=)` or the `delete` keyword, respectively.

```javascript
// Adding a new property
person.job = "Developer";

// Deleting an existing property
delete car.year;
```

### Special Data Types and Exceptions

- `Null`: Represents the intentional absence of any object value.
- `undefined` : Represents a variable that has been declared but has not yet been assigned a value.
- `Nan`(Not a Number): Represents a value that is not a valid number.
- `Infinity` and `-Infinity`: Represent positive and negative infinity, respectively.

```javascript
let emptyValue = null;
let undefinedValue;
let result = "hello" / 5; // NaN
let positiveInfinity = Infinity;
let negativeInfinity = -Infinity;
```

## Resources for Data Types

[![Video Thumbnail](https://img.youtube.com/vi/qpU3WIqRz9I/0.jpg)](https://youtu.be/qpU3WIqRz9I?si=LfxKqjlXMp3rxesV)

# Understanding Variable Scope in JavaScript

## **let**, **var**, and **const**

### let

The let keyword is used to declare a variable that can be reassigned a new value. Variables declared with let have block scope, meaning they are only accessible within the block in which they are defined.

```javascript
let age = 30;
age = 35; // Valid: Variable can be reassigned

{
  let name = "John";
  console.log(name); // Output: John
}

console.log(name); // Error: name is not defined
```

### var

The `var` keyword is the older way of declaring variables in JavaScript. Variables declared with `var` have function scope or global scope, depending on where they are declared. Unlike `let`, variables declared with `var` can be redeclared and reassigned within the same scope.Var have Function level scope.

```javascript
var count = 10;
var count = 20; // Valid: Variable can be redeclared

function greet() {
  var message = "Hello";
  console.log(message); // Output: Hello
}

console.log(message); // Error: message is not defined
```

Don't know about **functions** ? we will talk about that later. For now just understand Functions in JavaScript are blocks of code that can be defined once and executed multiple times. They encapsulate a set of instructions and can accept input parameters, perform computations, and return results.

### const

The `const` keyword is used to declare a constant variable, which cannot be reassigned a new value once it has been initialized. Variables declared with `const` must be initialized at the time of declaration.

```javascript
const pi = 3.14;
pi = 3.14159; // Error: Assignment to constant variable
```

In summary ,

- Use `let` for variables that may change their value over time and have block scope.
  -Use `var` sparingly, as it has function scope or global scope and can lead to unexpected behavior.
  -Use `const` for variables that should not be reassigned and have block scope.

Remember to choose the appropriate variable declaration based on the intended use and scope of the variable in your JavaScript code.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/yY0bKZNYmJs/0.jpg)](https://youtu.be/yY0bKZNYmJs?si=zvAWn6UPObSxihUi)

# Operators

Operators in JavaScript are symbols or keywords that perform operations on operands (variables or values). They are used to perform arithmetic, comparison, logical, and assignment operations

### Arithmetic Operators

Arithmetic operators are used to perform mathematical calculations.

- **Addition (+):** Adds two operands.
- **Subtraction (-):** Subtracts the second operand from the first.
- **Multiplication (\*):** Multiplies two operands.
- **Division (/):** Divides the first operand by the second.
- **Remainder (%):** Returns the remainder of the division of two operands.
- **Exponentiation (\*\*):** Raises the first operand to the power of the second.

```javascript
let a = 5;
let b = 3;
console.log(a + b); // Output: 8
console.log(a - b); // Output: 2
console.log(a * b); // Output: 15
console.log(a / b); // Output: 1.6666666666666667
console.log(a % b); // Output: 2
console.log(a ** b); // Output: 125
```

### Comparison Operators

Comparison operators are used to compare two values and return a Boolean result.

- **Equal (`==`):** Checks if two operands are equal.
- **Not Equal (`!=`):** Checks if two operands are not equal.
- **Strict Equal (`===`):** Checks if two operands are equal and of the same type.
- **Strict Not Equal (`!==`):** Checks if two operands are not equal and/or not of the same type.
- **Greater Than (`>`):** Checks if the left operand is greater than the right.
- **Less Than (`<`):** Checks if the left operand is less than the right.
- **Greater Than or Equal (`>=`):** Checks if the left operand is greater than or equal to the right.
- **Less Than or Equal (`<=`):** Checks if the left operand is less than or equal to the right.

```javascript

// Output: false
console.log("apple" == "Apple");\

// Output: true
console.log(3 == "3");

// Output: false
console.log(3 === "3");

// Output: true
console.log(10 >= "10");

// Output: true
console.log(null == undefined);

// Output: false
console.log(NaN === NaN);

// Output: false
console.log("cat" > "dog");

// Output: false
console.log([] == []);

// Output: true
console.log(0 == false);

// Output: false
console.log(0 === false);
```

### Explanation of Outputs

1. **console.log("apple" == "Apple");**

   - Explanation: The `==` operator performs type coercion( converting both operands to the same type before comparison) In this case, both operands are strings, but they differ in case. JavaScript is case-sensitive, so `"apple"` is not equal to `"Apple"`.
   - Expected Output: false

2. **console.log(3 == "3");**

   - Explanation: Similar to the previous example, the `==` operator performs type coercion. JavaScript converts the string `"3"` to a number before comparison, so `3` is equal to `3`.
   - Expected Output: true

3. **console.log(3 === "3");**

   - Explanation: The `===` operator performs strict equality comparison without type coercion. Since the types of the operands are different (`number` and `string`), they are not equal.
   - Expected Output: false

4. **console.log(10 >= "10");**

   - Explanation: The `>=` operator performs type coercion, converting the string `"10"` to a number before comparison. So, `10` is greater than or equal to `10`.
   - Expected Output: true

5. **console.log(null == undefined);**

   - Explanation: `null` and `undefined` are loosely equal (they are equal without type coercion), according to JavaScript's specification.
   - Expected Output: true

6. **console.log(NaN === NaN);**

   - Explanation: `NaN` is a special value in JavaScript representing "Not-a-Number". Surprisingly, `NaN` is not equal to itself, even in strict equality comparison.
   - Expected Output: false

7. **console.log("cat" > "dog");**

   - Explanation: Strings are compared based on their Unicode code points. The Unicode code point for `"c"` is lower than `"d"`, so `"cat"` is not greater than `"dog"`.
   - Expected Output: false

8. **console.log([] == []);**

   - Explanation: Arrays in JavaScript are reference types, and the `==` operator compares references, not the content of arrays. Two separate arrays will never be equal.
   - Expected Output: false

9. **console.log(0 == false);**

   - Explanation: In JavaScript, `0` is loosely equal to `false`. Both are falsy values, so they are considered equal without type coercion.
   - Expected Output: true

10. **console.log(0 === false);**
    - Explanation: The `===` operator performs strict equality comparison without type coercion. Since the types of the operands are different (`number` and `boolean`), they are not equal.
    - Expected Output: false

### Logical Operators

Logical operators are used to perform logical operations on boolean values. JavaScript supports three main logical operators: `&&` (AND), `||` (OR), and `!` (NOT).

- **AND (`&&`)**: Returns `true` if both operands are `true`, otherwise returns `false`.

  ```javascript
  const x = true;
  const y = false;
  console.log(x && y); // Output: false
  ```

- **OR (`||`)**: Returns `true` if either of the operands is `true`, otherwise returns `false`.

  ```javascript
  const a = true;
  const b = false;
  console.log(a || b); // Output: true
  ```

- **NOT (`!`)**: Returns `true` if the operand is `false`, and vice versa

```javascript
const value = false;
console.log(!value); // Output: true
```

### Assignment Operators

Assignment operators are used to assign values to variables. In JavaScript, the basic assignment operator is `=`. Additionally, there are compound assignment operators like `+=`, `-=`.

- **Basic Assignment (`=`):** Assigns the value on the right to the variable on the left.
  ```javascript
  let x = 5;
  let y = 10;
  ```
- **Compound Assignment (`+=`, `-=`):** Combines an arithmetic operation with the assignment.

```javascript
let a = 5;
a += 3; // equivalent to a = a + 3
console.log(a); // Output: 8

let b = 10;
b -= 5; // equivalent to b = b - 5
console.log(b); // Output: 5
```

### Bitwise Operators

Bitwise operators perform operations on the binary representation of numeric values.

**Note:** It's important to understand binary representations before diving into bitwise operators.

- **Bitwise AND (`&`)**: Returns a 1 in each bit position if both operands have a 1 in that position.
- **Bitwise OR (`|`)**: Returns a 1 in each bit position if either operand has a 1 in that position.
- **Bitwise XOR (`^`)**: Returns a 1 in each bit position if only one of the operands has a 1 in that position.
- **Bitwise NOT (`~`)**: Inverts the bits of its operand.
- **Left Shift (`<<`)**: Shifts the bits of the first operand to the left by the number of positions specified by the second operand.
- **Sign-propagating Right Shift (`>>`)**: Shifts the bits of the first operand to the right by the number of positions specified by the second operand.
- **Zero-fill Right Shift (`>>>`)**: Shifts the bits of the first operand to the right by the number of positions specified by the second operand. Zeros are shifted in from the left.

```javascript
let x = 5; // Binary representation: 0101
let y = 3; // Binary representation: 0011

console.log(x & y); // Bitwise AND: 0101 & 0011 = 0001 (1)
console.log(x | y); // Bitwise OR:  0101 | 0011 = 0111 (7)
console.log(x ^ y); // Bitwise XOR: 0101 ^ 0011 = 0110 (6)
console.log(~x); // Bitwise NOT: ~0101 = 1010 (-6 in 2's complement)
console.log(x << 1); // Left Shift: 0101 << 1 = 1010 (10)
console.log(x >> 1); // Right Shift: 0101 >> 1 = 0010 (2)
console.log(x >>> 1); // Zero-fill Right Shift: 0101 >>> 1 = 0010 (2)
```

### Comments

Comments are used to add explanatory notes to JavaScript code. JavaScript supports both single-line and multi-line comments.

```javascript
// This is a single-line comment

/*
This is a
multi-line comment
*/
```

### Resources for Operators

[![Video Thumbnail](https://img.youtube.com/vi/lsV8JQgSW1s/0.jpg)](https://youtu.be/lsV8JQgSW1s?si=MZ4XQUaL69VQXbzf)

[![Video Thumbnail](https://img.youtube.com/vi/mesu75PTDC8/0.jpg)](https://youtu.be/mesu75PTDC8?si=Z0Xgu8vY7LUK7zvD)

# Conditional Statements (if-else, switch):

Conditional statements are used to execute different actions based on different conditions.

### if-else Statement:

The `if-else` statement executes a block of code if a specified condition is true and another block of code if the condition is false.

```javascript
let x = 10;

if (x > 5) {
  console.log("x is greater than 5");
} else {
  console.log("x is not greater than 5");
}
```

### Ternary Operator

The ternary operator, also known as the conditional operator, is a concise way to write conditional statements in JavaScript. It is often used as a shortcut for simple `if...else` statements.

**Syntax**

```md
condition ? expressionIfTrue : expressionIfFalse
```

**Example**

```javascript
const age = 20;
const message = age >= 18 ? "You are an adult" : "You are a minor";
console.log(message); // Output: You are an adult
```

### Explanation

In the example above:

- The condition `age >= 18` checks if the age is greater than or equal to 18.
- If the condition is true, the expression `'You are an adult'` is evaluated.
- If the condition is false, the expression `'You are a minor'` is evaluated.
- The result of the ternary operator is then assigned to the variable `message`.

### switch Statement:

The `switch` statement evaluates an expression, matching the expression's value to a case clause, and executes statements associated with that case.

```javascript
let fruit = "Apple";

switch (fruit) {
  case "Banana":
    console.log("Banana is yellow.");
    break;
  case "Apple":
    console.log("Apple is red.");
    break;
  default:
    console.log("Unknown fruit.");
}
//output : Apple is red.
```

**Explanation**

The switch statement checks the value of `fruit` variable and executes the code block associated with the matching case. If no match is found, the code block under default is executed.

**note :**
"Don't worry if you're not familiar with the `break` statement yet; we'll delve into its functionality shortly in our study."

**Question:** What will be the output of the above code snippet? What happens if the fruit variable is set to "Banana"?

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/s5Lu4QTjeL0/0.jpg)](https://youtu.be/s5Lu4QTjeL0?si=fRfiRRT2P0iYS3JG)

[![Video Thumbnail](https://img.youtube.com/vi/SJPsOFfvEQA/0.jpg)](https://youtu.be/SJPsOFfvEQA?si=YhuKhdqNEbhLWq0b)

# Loops (for, while, do-while):

Loops are fundamental in programming as they allow us to execute a block of code repeatedly. JavaScript provides several types of loops, each with its own unique characteristics and use cases

### for Loop

The `for` loop is commonly used when the number of iterations is known or when iterating over arrays.

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

**Explanation**

In the above example, the loop initializes i to 0, checks if i is less than 5, executes the loop body, and increments i by 1 in each iteration.

**Question:** How many times will the loop execute in the above code snippet? What will be the output?

**Answer:** The loop will execute 5 times, printing numbers from 0 to 4. The output will be:

```md
0
1
2
3
4
```

### while Loop

The `while` loop is useful when the number of iterations is unknown but a condition needs to be met for the loop to continue.

```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

**Explanation**

The while loop checks the condition before each iteration. It executes the loop body as long as the condition (i < 5) evaluates to true.

**Question:** What happens if the condition in the while loop is always true? How can you prevent an infinite loop?

**Answer:** If the condition in a `while` loop is always true, the loop will continue to execute indefinitely, resulting in an _infinite_ loop. This can cause the program to become unresponsive or crash. To prevent an infinite loop, ensure that the loop's condition eventually becomes false or use control flow statements like `break` to exit the loop under certain conditions.

And remember, if you find yourself accidentally creating an infinite loop, don't worry! It happens to the best of us. Take a moment to reflect, debug, and maybe even try intentionally creating one just to see what happens. Let your PC have some fun too!

### do-while Loop

The `do-while` loop is similar to the `while` loop, but it always executes the loop body at least once before checking the condition.

```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

**Explanation**

In the above example, the loop body is executed once before the condition `(i < 5)` is evaluated. If the condition is true, the loop continues to execute.

**Question:** How is the behavior of a do-while loop different from that of a while loop? Provide an example where this difference is significant.

**Answer:** Unlike the while loop, the do-while loop always executes the loop body at least once, regardless of the condition's initial value.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/XKyyM1VWtUE/0.jpg)](https://youtu.be/XKyyM1VWtUE?si=jQ__72E7GaspMG8a)

[![Video Thumbnail](https://img.youtube.com/vi/drEjyBSu33w/0.jpg)](https://youtu.be/drEjyBSu33w?si=CSD1__KvIwsJ2gG_)

# Break and Continue Statements

`break` and `continue` statements are used to control the flow of loops. These are also called _Jump_ Statements

### break Statement

The break statement terminates the current loop, switch, or label statement and transfers program control to the statement following the terminated statement.

```javascript
for (let i = 0; i < 10; i++) {
  if (i === 5) {
    break;
  }
  console.log(i);
}
```

```md
0
1
2
3
4
```

**Explanation**

- The `for` loop initializes `i` to `0` and iterates as long as `i` is less than `10`.
- In each iteration, it checks if `i` is equal to `5`.
- When `i` is `5`, the `break` statement is executed, which terminates the loop immediately.
- Therefore, only the values of `i` from `0` to `4` are printed using `console.log(i)`.

### Continue Statement

The `continue` statement is used within loops in JavaScript to skip the current iteration of the loop and proceed to the next iteration. It is commonly used to avoid executing certain code or processing specific elements within a loop.

```javascript
for (let i = 0; i < 5; i++) {
  if (i === 2) {
    continue; // Skip the current iteration when i is 2
  }
  console.log(i);
}
```

### Explanation

In the example above:

- We have a for loop that iterates from 0 to 4.
- Inside the loop, we use an if statement to check if the current value of i is 2.
- If i is 2, the continue statement is executed, which skips the current iteration of the loop.
- As a result, when i is 2, the console.log(i) statement is skipped, and the loop proceeds to the next iteration.
- The output of the loop is 0, 1, 3, and 4.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/Y1cpFsXrEgY/0.jpg)](https://youtu.be/Y1cpFsXrEgY?si=-m29Sh0C5KWXFXyp)

# JavaScript Functions

Functions are reusable blocks of code that perform a specific task or calculate a value. They allow for modular programming and help in organizing code for better readability and maintainability.

### What are Functions?

A function is a block of code that performs a specific task or calculates a value. It consists of a set of statements that are executed when the function is called. Functions can take inputs, known as parameters, and can optionally return a value.

### Declaring Functions

A function in JavaScript can be declared using the `function` keyword followed by the function name, parentheses `()`, and curly braces `{}` to define the function body.

```javascript
function greet() {
  console.log("Hello, world!");
}
```

### Calling Functions

To execute a function and perform its task, you need to call it by using its name followed by parentheses `()`.

```javascript
greet(); // Output: Hello, world!
```

### Function Parameters

Functions can accept inputs, called parameters, which are specified within the parentheses `()`. These parameters allow functions to perform tasks with different values.

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}

greet("Alice"); // Output: Hello, Alice!
```

### Return Statement

A function can optionally return a value using the `return` statement. This allows the function to provide a result that can be used elsewhere in the code.

```javascript
function add(a, b) {
  return a + b;
}

let result = add(3, 5);
console.log(result); // Output: 8
```

### Anonymous Functions

Anonymous functions, also known as function expressions, are functions without a name. They are often used as arguments to other functions or assigned to variables.

```javascript
let greet = function () {
  console.log("Hello, world!");
}; // Anonymous function on R.H.S

greet(); // Output: Hello, world!
```

### Arrow Functions

Arrow functions provide a concise syntax for writing functions, especially when the function body consists of a single expression. They are denoted by the arrow `=>`and automatically bind this to the surrounding code.

```javascript
let greet = () => {
  console.log("Hello, world!");
};

greet(); // Output: Hello, world!

//Upper function is equivalent to this one:
function greet() {
  console.log("Hello, world!");
}
```

### Immediately Invoked Function

It is a JavaScript function that runs as soon as it defined. An `IIFE` (Immediately Invoked Function Expression) can be used for avoiding the variable hoisting from within the blocks. It allows the public access to methods while retaining the privacy for variables defined in the function.

IIFE is a design pattern that is also known as the **Self-Executing Anonymous Function**.

```javascript
(function () {
  const message = "Hello from IIFE!";
  console.log(message);
})();
```

### Exercise Time!

**Note:** Challenge yourself by attempting to solve these questions on your own before peeking at the answers! It's a great way to test your understanding and strengthen your problem-solving skills

**1. Question:** What will be the output of the code snippet?

```javascript
function greet(name) {
  return "Hello, " + name + "!";
}

let message = greet("Alice");
console.log(message);
```

**Answer and Explanation**

The output of the code snippet will be `Hello, Alice!`. Here's the explanation:

- The `greet` function takes a `name` parameter and returns a greeting message with the provided name.
- When `greet("Alice")` is called, the function returns `"Hello, Alice!"`, which is assigned to the variable `message`.
- Therefore, `message` contains the string `"Hello, Alice!"`, which is then logged to the console.

**2. Question :** What will be the output of the code snippet?

```javascript
function add(a, b) {
  return a + b;
}

function multiply(a, b) {
  return a * b;
}

let result = multiply(add(2, 3), 4);
console.log(result);
```

**Answer and Explanation**

The output of the code snippet will be `20`. Here's the explanation:

- The `add` function adds its two parameters (`2` and `3`) and returns the result `5`.
- The `multiply` function multiplies its two parameters (result of `add(2, 3)` and `4`) and returns the result `20`.
- Therefore, `result` is assigned the value `20`, which is then logged to the console.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/a_gwOwkbhZ0/0.jpg)](https://youtu.be/a_gwOwkbhZ0?si=QYyStZ3k3fBJculm)

[![Video Thumbnail](https://img.youtube.com/vi/9ksqBa8_txM/0.jpg)](https://youtu.be/9ksqBa8_txM?si=A2ma6YuPBlXaQ8cJ)

[![Video Thumbnail](https://img.youtube.com/vi/GAIbn16Iytc/0.jpg)](https://youtu.be/GAIbn16Iytc?si=VjkCnQc_Kf-bX9K8)

# JavaScript Scope and Closures

Scope and closures are fundamental concepts in JavaScript that determine the accessibility and lifetime of variables and functions within a program.

## Variable Scope

Variable scope refers to the region of code where a variable is accessible. In JavaScript, variables can have either global or local scope.

### Global Scope

Variables declared outside of any function have global scope, meaning they can be accessed from anywhere in the code.

```javascript
let globalVar = "I am a global variable";

function foo() {
  console.log(globalVar); // Output: I am a global variable
}

foo();
```

### Function Scope

Variables declared within a function have function scope, meaning they are accessible only within that function.

```javascript
function foo() {
  let localVar = "I am a local variable";
  console.log(localVar); // Output: I am a local variable
}

foo();
console.log(localVar); // Error: localVar is not defined
```

### Lexical Scope

Lexical scope refers to the ability of nested functions to access variables defined in their outer scope. JavaScript uses lexical scoping, also known as _static_ scoping.

```javascript
function outerFunction() {
  let outerVar = "I am from outer function";
  function innerFunction() {
    console.log(outerVar); // Output: I am from outer function
  }
  innerFunction();
}

outerFunction();
```

### Closures

A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In other words, a closure gives you access to an outer function's scope from an inner function. In JavaScript, closures are created every time a function is created, at function creation time.

**or**

Closures occur when an inner function retains access to variables from its outer scope even after the outer function has finished executing. They are formed when a function is defined within another function.

```javascript
function outerFunction() {
  let outerVar = "I am from outer function";
  function innerFunction() {
    console.log(outerVar); // Output: I am from outer function
  }
  return innerFunction;
}

let innerFunc = outerFunction();
innerFunc();
```

### Explanation

- The `outerFunction` is defined, which declares a variable `outerVar` and defines an inner function `innerFunction`.
- Within `outerFunction`, `innerFunction` is defined. This inner function has access to the variable `outerVar` due to lexical scoping rules in JavaScript.
- `outerFunction` returns the `innerFunction`. This means that the `innerFunction` retains access to the `outerVar` variable even after `outerFunction` has finished executing. This is the concept of closure.
- The returned `innerFunction` is assigned to the variable `innerFunc`.
- `innerFunc` is then called, which executes the `innerFunction` code.
- The `innerFunction` prints the value of `outerVar` to the console, which is `"I am from outer function"`.

In summary, the code demonstrates how inner functions can retain access to variables from their outer scope, even after the outer function has finished executing. This concept of closure allows for powerful and flexible programming patterns in JavaScript.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/cHHU0jXfjKY/0.jpg)](https://youtu.be/cHHU0jXfjKY?si=o-1zmddy9t1Rg5lI)

[![Video Thumbnail](https://img.youtube.com/vi/VaH09NXQZ58/0.jpg)](https://youtu.be/VaH09NXQZ58?si=trX-hTjjx4bcZTXZ)

# Working with Arrays

Arrays and objects are fundamental data structures in JavaScript that allow for the storage and manipulation of data.

### Creating Arrays

Arrays in JavaScript can be created using square brackets `[]` and can hold elements of any data type.

```javascript
let numbers = [1, 2, 3, 4, 5];
let fruits = ["apple", "banana", "orange"];
```

### Accessing Array Elements

Array elements can be accessed using square brackets `[]` with the index of the element.

```javascript
console.log(numbers[0]); // Output: 1
console.log(fruits[1]); // Output: banana
```

### Adding and Removing Elements

Elements can be added to the end of an array using the `push` method and removed using the `pop` method . These are inbuild methods in Javascript. Unlike other languages , You don't have to define it externally.

```javascript
fruits.push("grape"); // Adds 'grape' to the end of the array
console.log(fruits); // Output: ['apple', 'banana', 'orange', 'grape']

fruits.pop(); // Removes the last element from the array
console.log(fruits); // Output: ['apple', 'banana', 'orange']
```

## Array Methods in JavaScript

Below are detailed explanations of various array methods in JavaScript, along with examples and indications of whether they modify the original array or not:

### 1. `toString` Method (Does Not Modify):

The `toString` method converts an array to a string of comma-separated values.

```javascript
let fruits = ["apple", "banana", "orange"];
let result = fruits.toString();
console.log(result); // Output: apple,banana,orange
```

### 2. `join` Method (Does Not Modify):

The `join` method joins all elements of an array into a string.

```javascript
let fruits = ["apple", "banana", "orange"];
let result = fruits.join(" | ");
console.log(result); // Output: apple | banana | orange
```

### 3. `shift` Method (Modifies):

The `shift` method removes the first element from an array and returns that removed element.

```javascript
let fruits = ["apple", "banana", "orange"];
let removedElement = fruits.shift();
console.log(removedElement); // Output: apple
console.log(fruits); // Output: ['banana', 'orange']
```

### 4. `unshift` Method (Modifies):

The unshift method adds one or more elements to the beginning of an array and returns the new length of the array.

```javascript
let fruits = ["banana", "orange"];
let newLength = fruits.unshift("apple");
console.log(newLength); // Output: 3
console.log(fruits); // Output: ['apple', 'banana', 'orange']
```

### 5. `delete` Operator (Modifies):

The `delete` operator removes a specified element from an array but leaves a hole in the array.

```javascript
let fruits = ["apple", "banana", "orange"];
delete fruits[1];
console.log(fruits); // Output: ['apple', empty, 'orange']
```

Yes there will be no `fruits.delete()` , delete is used like this only!

### 6. `concat` Method (Does Not Modify):

The `concat` method merges two or more arrays and returns a new array.

```javascript
let fruits1 = ["apple", "banana"];
let fruits2 = ["orange", "grape"];
let result = fruits1.concat(fruits2);
console.log(result); // Output: ['apple', 'banana', 'orange', 'grape']
```

### 7. `slice` Method (Does Not Modify):

The `slice` method returns a shallow copy of a portion of an array into a new array object.

```javascript
let fruits = ["apple", "banana", "orange", "grape"];
let result = fruits.slice(1, 3); //3 excluded , content from index 1 to 2 will be there in output
console.log(result); // Output: ['banana', 'orange']
```

JavaScript provides several built-in methods for working with arrays, including `forEach`, `map`, `filter`, `reduce`, etc.

### 8. `splice` Method (Modifies):

The `splice` method changes the contents of an array by removing or replacing existing elements and/or adding new elements.

```javascript
let fruits = ["apple", "banana", "orange", "grape"];

// Starting at index 1 (banana), remove 2 elements (banana and orange)
// and insert 'kiwi' and 'melon' in their place
fruits.splice(1, 2, "kiwi", "melon");

console.log(fruits); // Output: ['apple', 'kiwi', 'melon', 'grape']
```

### 9. `reverse` Method (Modifies):

The `reverse` method reverses the elements of an array in place.

```javascript
let fruits = ["apple", "banana", "orange", "grape"];
fruits.reverse();
console.log(fruits); // Output: ['grape', 'orange
```

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/a_Bz5ciBHQ0/0.jpg)](https://youtu.be/a_Bz5ciBHQ0?si=yFLFlXygpVXc1vDC)

[![Video Thumbnail](https://img.youtube.com/vi/BLIrBThPTXc/0.jpg)](https://youtu.be/BLIrBThPTXc?si=RxjK1FPt5Y8HMd92)

[![Video Thumbnail](https://img.youtube.com/vi/QxA-KB2lKgk/0.jpg)](https://youtu.be/QxA-KB2lKgk?si=1L9V48cgK1M-S1z7)

## Modern Array Methods

Some Very Useful methods are there in javascript and you will use them a lot of time in your projects , That's why it is presented here in a different section

### 1. `map` Method (Does Not Modify):

The `map()` method creates a new array by applying a provided function to each element of the original array.

```javascript
let newArray = array.map(callback(currentValue, index , array) {
  // return modified value
});
```

- `callback` : A function to execute on each element.
- `currentValue` : The current element being processed in the array.
- `index`(optional) : The index of the current element being processed.
- `array`(optional) : The array `map()` was called upon.

```javascript
let numbers = [1, 2, 3, 4, 5];
let doubledNumbers = numbers.map(function (number) {
  return number * 2;
});
console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]
```

### 2. `filter` Method (Does Not Modify):

The `filter()` method creates a new array with all elements that pass a test implemented by the provided function.

```javascript
let newArray = array.filter(callback(currentValue, index, array) {
  // return true to keep the element, false otherwise
});
```

- `callback` : A function to execute on each element.
- `currentValue` : The current element being processed in the array.
- `index`(optional) : The index of the current element being processed.
- `array`(optional) : The array `filter()` was called upon.

```javascript
let numbers = [1, 2, 3, 4, 5];
let evenNumbers = numbers.filter(function (number) {
  return number % 2 === 0;
});
console.log(evenNumbers); // Output: [2, 4]
```

### 3. `reduce` Method (Does Not Modify):

The `reduce()` method applies a function against an accumulator and each element in the array to reduce it to a single value.

```javascript
let result = array.reduce(
  callback(accumulator, currentValue, index, array),
  initialValue
);
```

- `callback` : A function to execute on each element.
- `accumulator`: The accumulator accumulates the callback's return values.
- `currentValue` : The current element being processed in the array.
- `index`(optional) : The index of the current element being processed.
- `array`(optional) : The array ` reduce()` was called upon.
- `initialValue` (optional): A value to use as the first argument to the first call of the callback.

```javascript
let numbers = [1, 2, 3, 4, 5];
let sum = numbers.reduce(function (accumulator, currentValue) {
  return accumulator + currentValue;
}, 0);
console.log(sum); // Output: 15
```

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/bAUMuuRH99o/0.jpg)](https://youtu.be/bAUMuuRH99o?si=_5gUujs5s4lYKGZ2)

## Looping Through Arrays

Arrays can be looped through using the classical Javascript for loop or through some other methods discussed below

### 1. `forEach` Method:

The `forEach()` method executes a provided function once for each array element.

```javascript
array.forEach(callback(currentValue , index , array) {
  // function logic
});
```

- `callback` : A function to execute on each element.
- `currentValue` : The current element being processed in the array.
- `index`(optional) : The index of the current element being processed.
- `array`(optional) : The array `forEach()` was called upon.

```javascript
let numbers = [1, 2, 3, 4, 5];
// forEach method
numbers.forEach(function (number) {
  console.log(number); // Output: 1, 2, 3, 4, 5
});
```

### 2. `for...of` Loop:

The `for...of` loop is used to iterate over iterable objects, such as arrays, strings, maps, sets, and more, to execute a block of code for each distinct element of the iterable.

```javascript
for (variable of iterable) {
  // code block to be executed
}
```

```javascript
let fruits = ["apple", "banana", "orange"];

for (let fruit of fruits) {
  console.log(fruit);
}
// Output:
// apple
// banana
// orange
```

In this example, the `for...of` loop iterates over each element in the `fruits` array, assigning each element to the `fruit` variable, and then logs each `fruit` to the console.

### 3. `for...in` Loop:

The `for...in` loop is used to iterate over the properties of an object, including enumerable properties from the object's prototype chain.

```javascript
for (variable in object) {
  // code block to be executed
}
```

```javascript
let person = { name: "John", age: 30, city: "New York" };

for (let key in person) {
  console.log(`${key}: ${person[key]}`);
}
// Output:
// name: John
// age: 30
// city: New York
```

In this example, the `for...in` loop iterates over each property in the `person` object, assigning each property key to the `key` variable, and then logs the property key along with its corresponding value to the console.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/YWyr7Nug2oc/0.jpg)](https://youtu.be/YWyr7Nug2oc?si=E8wJlrGgy5O94WTM)

# Error Handling in JavaScript

Error handling in JavaScript allows you to gracefully manage and recover from runtime errors or unexpected situations in your code.

### `Try-Catch` Statement

The `try...catch` statement is used to handle exceptions in JavaScript. You can wrap code that might throw an error inside a `try` block, and catch and handle any errors that occur in the corresponding `catch` block.

```javascript
try {
  // Code that might throw an error
  let result = someFunction();
  console.log(result);
} catch (error) {
  // Code to handle the error
  console.error("An error occurred:", error.message);
}
```

### Error Objects

JavaScript provides built-in error objects that represent different types of errors that can occur during the execution of your code. These error objects include `Error`, `SyntaxError`, `TypeError`, `ReferenceError`, and more.

```javascript
try {
  // Code that might throw an error
  throw new Error("Custom error message");
} catch (error) {
  // Code to handle the error
  console.error("An error occurred:", error.message);
}
```

In this example, if an error occurs within the `try` block or if the `throw` statement is explicitly called, the execution of the `try` block is interrupted, and the control is transferred to the `catch` block, where you can handle the error.

The `throw` statement is used to throw a user-defined exception or a predefined JavaScript error. It interrupts the execution of the script. The `throws` keyword is not a part of JavaScript; it is typically used in function declarations to indicate the types of exceptions that the function may throw, but JavaScript itself does not enforce this.

Error handling is an essential aspect of writing robust and reliable JavaScript code, especially when dealing with asynchronous operations, external APIs, or user input. Understanding how to use `try...catch` statements and error objects can help you write code that gracefully handles errors and prevents unexpected crashes.

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/WRNBQCl_cPU/0.jpg)](https://youtu.be/WRNBQCl_cPU?si=rYcMIKJl-dHXujt-)

[![Video Thumbnail](https://img.youtube.com/vi/uOQBGKfldIg/0.jpg)](https://youtu.be/uOQBGKfldIg?si=xKzWPTI8GTsROrD3)

# Javascript in the browser

Javascript was initially created to make web pages alive . JS can be written right in a web page's HTML to make it interactive .The browser has an embedded engine called the Javascript engine or the Javascript runtime.

JavaScript' ability in the browser is very limited to protect the user's safety. for example a webpage on http://google.com Cannot Access http://codeswear.com and steal information from there

## Interactivity with browser

### `alert()`

The `alert()` method displays a dialog box with a specified message and an OK button. It is commonly used to alert users about important information or to display error messages.

```javascript
alert("Hello, world!");
```

### `prompt()`

The `prompt()` method displays a dialog box that prompts the user for input. It includes a text field where the user can enter data. The method returns the text entered by the user or `null` if the user clicks the Cancel button.

```javascript
const name = prompt("Please enter your name:", "John Doe"); // 2nd parameter is for default value
console.log("Hello, " + name + "!");
```

### `confirm()`

The `confirm()` method displays a dialog box with a message and two buttons: OK and Cancel. It is commonly used to ask users for confirmation before performing an action.

```javascript
const result = confirm("Are you sure you want to delete this item?");
if (result === true) {
  // Delete the item
  console.log("Item deleted.");
} else {
  // Cancel the deletion
  console.log("Deletion canceled.");
}
```

### Resources

[![Video Thumbnail](https://img.youtube.com/vi/540NIdeKW3I/0.jpg)](https://youtu.be/540NIdeKW3I?si=Wtyc_L0EuSkL7Gkw)

# What is DOM ?

The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of an HTML document as a tree-like structure, where each node represents an element or an attribute of the document. The DOM provides a way for JavaScript to interact with and manipulate the structure, content, and style of web pages.

**Example HTML Document**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>DOM Manipulation Examples</title>
  </head>
  <body>
    <div id="container">
      <h1>Welcome to DOM Manipulation</h1>
      <p class="content">
        This is a sample HTML document for DOM manipulation.
      </p>
      <button id="btn">Click me!</button>
    </div>
  </body>
</html>
```

**note** : Go through this HTML Document , We will be using this document for further learnings with DOM

## Accessing DOM Elements

JavaScript provides several methods to access DOM elements, allowing you to select elements based on their ID, class, tag name, or relationship with other elements.

### Example: Accessing Elements by ID

```javascript
const container = document.getElementById("container");
console.log(container); // Output: <div id="container">...</div>
```

So , certain methods to select HTML elements are as follows :

### document.getElementById()

The `getElementById()` method returns the element that has the specified ID attribute.

```javascript
const container = document.getElementById("container");
console.log(container); // Output: <div id="container">...</div>
```

### document.getElementsByClassName()

The `getElementsByClassName()` method returns a collection of all elements in the document with the specified class name.

```javascript
const paragraphs = document.getElementsByClassName("content");
console.log(paragraphs); // Output: HTMLCollection [ <p class="content">...</p> ]
```

### document.getElementsByTagName()

The `getElementsByTagName()` method returns a collection of all elements in the document with the specified tag name.

```javascript
const headings = document.getElementsByTagName("h1");
console.log(headings); // Output: HTMLCollection [ <h1>Welcome to DOM Manipulation</h1> ]
```

### document.querySelector()

The `querySelector()` method returns the first element that matches a specified CSS selector in the document.

```javascript
const button = document.querySelector("#btn");
console.log(button); // Output: <button id="btn">Click me!</button>
```

### document.querySelectorAll()

The `querySelectorAll()` method returns a static (not live) NodeList representing a list of elements that match the specified group of selectors.

```javascript
const elements = document.querySelectorAll(".content");
console.log(elements); // Output: NodeList [ <p class="content">...</p> ]
```

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>DOM Insertion Examples</title>
  </head>
  <body>
    <div id="parent">
      <h1>Parent Element</h1>
      <p>This is the parent element.</p>
      <div id="reference">Reference Element</div>
      <div id="toReplace">Element to Replace</div>
    </div>
  </body>
</html>
```

## Insertion Methods in DOM

### innerText

The `innerText` property sets or returns the text content of the specified node and all its descendants

```javascript
const element = document.getElementById("example");
element.innerText = "New text content"; // Expected Output: The text content of the <h1> element is changed to "New text content"
```

### innerHTML

The `innerHTML` property sets or returns the HTML content (including the HTML tags) of an element.

```javascript
const element = document.getElementById("example");
element.innerHTML = "<b>New</b> HTML content"; // Expected Output: The HTML content of the <h1> element is changed to "<b>New</b> HTML content"
```

### appendChild

The `appendChild()` method appends a node as the last child of a specified parent node.

```javascript
const parent = document.getElementById("parent");
const child = document.createElement("div");
child.textContent = "New child node";
parent.appendChild(child); // Expected Output: A new <div> element with the text "New child node" is appended to the end of the parent element
```

### insertBefore

The `insertBefore()` method inserts a node before a specified child node in the parent element.

```javascript
const parent = document.getElementById("parent");
const newChild = document.createElement("div");
newChild.textContent = "New child node";
const referenceNode = document.getElementById("reference");
parent.insertBefore(newChild, referenceNode); // Expected Output: A new <div> element with the text "New child node" is inserted before the element with ID "reference"
```

### insertAdjacentHTML

The `insertAdjacentHTML()` method inserts HTML text as a child, before, or after the specified element.

```javascript
const element = document.getElementById("example");
element.insertAdjacentHTML("beforeend", "<p>New HTML content</p>"); // Expected Output: A new <p> element with the text "New HTML content" is inserted as a child of the <h1> element
```

### createTextNode

The `createTextNode()` method creates a new Text node with the specified text.

```javascript
const textNode = document.createTextNode("New text node");
const parent = document.getElementById("parent");
parent.appendChild(textNode); // Expected Output: A new Text node with the text "New text node" is appended to the parent element
```

# Event Handling in JavaScript

Event handling in JavaScript allows you to respond to user interactions or system events in web applications. With event handling, you can execute JavaScript code in response to events such as clicks, keypresses, mouse movements, and more.

## Adding Event Listeners

The most common way to handle events in JavaScript is by adding event listeners to DOM elements. Event listeners "listen" for a specific event to occur on an element and execute a callback function when the event occurs.

**syntax**

```javascript
element.addEventListener(eventType, callbackFunction);
```

**Example:**

```javascript
const button = document.getElementById("myButton");

button.addEventListener("click", function () {
  console.log("Button clicked!");
});
```

### Event Object

When an event occurs, JavaScript creates an event object that contains information about the event. This event object is passed to the event handler function as an argument, allowing you to access details such as the event type, target element, mouse coordinates, and more.

```javascript
document.addEventListener("click", function (event) {
  console.log("Clicked at:", event.clientX, event.clientY);
});
```

### Event Propagation

In the DOM, events propagate or "bubble" from the target element to its ancestors. Additionally, events can also "capture" from the root of the document down to the target element. Understanding event propagation is crucial for handling events effectively, especially when dealing with nested elements.

```javascript
const parent = document.getElementById("parent");

parent.addEventListener("click", function () {
  console.log("Parent clicked!");
});

const child = document.getElementById("child");

child.addEventListener("click", function (event) {
  event.stopPropagation(); // Prevents event from bubbling up to parent
  console.log("Child clicked!");
});
```

### Removing Event Listeners

To remove an event listener from an element, you can use the `removeEventListener()` method.

**Syntax**

```javascript
element.removeEventListener(eventType, callbackFunction);
```

**Example**

```javascript
const button = document.getElementById("myButton");
const handleClick = function () {
  console.log("Button clicked!");
};

button.addEventListener("click", handleClick);

// Later, remove the event listener
button.removeEventListener("click", handleClick);
```

Certainly! When you define the callback function directly inside the `addEventListener` call, a new function is created every time the `addEventListener` line is executed. Even if the function has the same code, it's a different instance each time. Consequently, when you later call `removeEventListener`, you need to pass the exact same function instance that was originally added. If you define the function externally and then reference it in both `addEventListener` and `removeEventListener`, you're ensuring that the same function instance is used for both operations. This ensures that the event listener is removed successfully, preventing memory leaks and unexpected behavior.

## Additional Events

### 1. keydown

The `keydown` event occurs when a key is pressed down.

```javascript
document.addEventListener("keydown", function (event) {
  console.log("Key pressed:", event.key);
});
```

### 2. submit

The `submit` event occurs when a form is submitted.

```javascript
const form = document.getElementById("myForm");

form.addEventListener("submit", function (event) {
  event.preventDefault(); // Prevents the form from submitting
  console.log("Form submitted!");
});
```

Event handling in JavaScript provides a wide range of events that you can use to create interactive web applications. In addition to the events mentioned above, there are many more events available such as `mouseover`, `mouseout`, `focus`, `blur`, `change`, `scroll`, and more. Experiment with different events to enhance the interactivity and functionality of your web applications.

# Asynchronous JavaScript

### setTimeout

`setTimeout` is a JavaScript function used to schedule a function or piece of code to run after a specified delay (in milliseconds).

**Syntax**

```javascript
setTimeout is a JavaScript function used to schedule a function or piece of code to run after a specified delay (in milliseconds).
```

- **callback:** The function to execute after the delay.
- **delay:** The number of milliseconds to wait before executing the callback.

```javascript
callback: The function to execute after the delay.
delay: The number of milliseconds to wait before executing the callback.
```

### setInterval

`setInterval` is a JavaScript function used to repeatedly execute a function or piece of code at specified intervals.

```javascript
let count = 0;
function increment() {
  count++;
  console.log("Count:", count);
}

const intervalId = setInterval(increment, 1000); // Output: Count: 1, Count: 2, Count: 3, ...
```

### clearInterval

To stop the repeated execution of `setInterval`, you can use the `clearInterval` function by passing the interval ID returned by setInterval.

```javascript
let count = 0;
function increment() {
  count++;
  console.log("Count:", count);
  if (count === 5) {
    clearInterval(intervalId);
  }
}

const intervalId = setInterval(increment, 1000); // Output: Count: 1, Count: 2, Count: 3, Count: 4, Count: 5
```

### Callback Functions

Callback functions are functions that are passed as arguments to other functions and are executed later in response to some event or asynchronous operation completion.

```javascript
function fetchData(callback) {
  // Simulate fetching data asynchronously
  setTimeout(() => {
    const data = "Data fetched!";
    callback(data);
  }, 1000);
}

function processData(data) {
  console.log("Processing:", data);
}

fetchData(processData); // Output: Processing: Data fetched!
```

### Callback Hell

Callback hell, also known as pyramid of doom, occurs when multiple nested callback functions are used, leading to code that is difficult to read and maintain.

```javascript
function fetchData(callback) {
  setTimeout(() => {
    const data = "Data fetched!";
    callback(data);
  }, 1000);
}

function processData(data, callback) {
  setTimeout(() => {
    const processedData = `${data} Processed!`;
    callback(processedData);
  }, 1000);
}

function displayData(data) {
  console.log("Displaying:", data);
}

fetchData(function (data) {
  processData(data, function (processedData) {
    displayData(processedData);
  });
});
```

### Promises

Promises provide a cleaner alternative to callbacks for handling asynchronous operations. They represent a value that may be available now, or in the future, or never.

```javascript
function fetchData() {
  return new Promise((resolve, reject) => {
    // Simulate fetching data asynchronously
    setTimeout(() => {
      const data = "Data fetched!";
      resolve(data);
    }, 1000);
  });
}

function processData(data) {
  return new Promise((resolve, reject) => {
    // Simulate processing data asynchronously
    setTimeout(() => {
      const processedData = `${data} Processed!`;
      resolve(processedData);
    }, 1000);
  });
}

fetchData()
  .then(processData)
  .then((data) => {
    console.log("Displaying:", data); // Output: Displaying: Data fetched! Processed!
  })
  .catch((error) => {
    console.error("Error:", error);
  });
```

### Explanation:

1. **`fetchData` Function:**

   - This function simulates fetching data asynchronously.
   - It returns a `Promise` object.
   - Inside the `Promise` constructor, there's a function with two arguments: `resolve` and `reject`.
   - Inside the function, there's a `setTimeout` function that waits for 1000 milliseconds (1 second) before executing its callback.
   - After 1000 milliseconds, it resolves the promise with the string `'Data fetched!'`.

2. **`processData` Function:**

   - This function simulates processing the fetched data asynchronously.
   - It also returns a `Promise` object.
   - Similar to `fetchData`, it has a `setTimeout` function inside the `Promise` constructor.
   - After 1000 milliseconds, it resolves the promise with the processed data, which is the original data concatenated with the string `' Processed!'`.

3. **Promise Chain:**

   - We call the `fetchData` function, which returns a promise.
   - We chain a `.then()` method to the promise returned by `fetchData`.
   - Inside the `.then()` method, we pass the `processData` function as a callback.
   - This means that when the data is successfully fetched (promise resolved), the `processData` function will be called with the fetched data.
   - The `processData` function returns another promise, which allows us to chain another `.then()` method.
   - Inside the second `.then()` method, we log the processed data to the console.
   - We also chain a `.catch()` method to handle any errors that might occur during the process.

4. **Error Handling:**
   - If an error occurs at any stage of the promise chain (either during data fetching or processing), it will be caught by the `.catch()` method.
   - In this example, we simply log the error message to the console using `console.error()`.

### Async/Await

Async functions and the await keyword provide a more concise and synchronous-looking way to work with promises. Async functions implicitly return a promise and can use the await keyword to wait for the resolution of another promise.

```javascript
async function fetchData() {
  return new Promise((resolve, reject) => {
    // Simulate fetching data asynchronously
    setTimeout(() => {
      const data = "Data fetched!";
      resolve(data);
    }, 1000);
  });
}

async function processData(data) {
  return new Promise((resolve, reject) => {
    // Simulate processing data asynchronously
    setTimeout(() => {
      const processedData = `${data} Processed!`;
      resolve(processedData);
    }, 1000);
  });
}

async function displayData() {
  try {
    const data = await fetchData();
    const processedData = await processData(data);
    console.log("Displaying:", processedData); // Output: Displaying: Data fetched! Processed!
  } catch (error) {
    console.error("Error:", error);
  }
}

displayData();
```

### Explanation:

1. **`fetchData` Function:**

   - This is an asynchronous function declared with the `async` keyword, which means it returns a promise.
   - Inside the function, a promise is created using the `Promise` constructor, which simulates fetching data asynchronously.
   - A `setTimeout` function is used to delay the resolution of the promise by 1000 milliseconds (1 second).
   - After the delay, the promise is resolved with the string `'Data fetched!'`.

2. **`processData` Function:**

   - Similar to `fetchData`, this is an asynchronous function declared with the `async` keyword.
   - It also returns a promise.
   - Inside the function, a promise is created using the `Promise` constructor to simulate processing data asynchronously.
   - Again, a `setTimeout` function is used to delay the resolution of the promise by 1000 milliseconds.
   - After the delay, the promise is resolved with the processed data, which is the original data concatenated with the string `' Processed!'`.

3. **`displayData` Function:**

   - This is another asynchronous function declared with the `async` keyword.
   - Inside the function, a try-catch block is used to handle potential errors.
   - `await` is used to wait for the promises returned by `fetchData` and `processData` to resolve.
   - Once both promises are resolved, the processed data is logged to the console.

4. **Promise Execution:**
   - When `displayData` is called, it waits for `fetchData` to resolve using `await`.
   - After `fetchData` resolves, it passes the fetched data to `processData` using `await`.
   - When `processData` resolves, the processed data is obtained, and the execution continues.
   - Any errors that occur during the execution of `fetchData`, `processData`, or during the `await` statements are caught by the catch block and logged to the console.

This code demonstrates how async/await can be used to write asynchronous code in a more synchronous and readable manner in JavaScript.

# ES6 Features

### 1. Let and Const

**Let**

The `let` keyword allows you to declare block-scoped variables that can be reassigned.

```javascript
let x = 10;
if (true) {
  let y = 20;
  console.log(x); // Output: 10
  console.log(y); // Output: 20
}
console.log(x); // Output: 10
console.log(y); // Error: y is not defined
```

**Const**

The `const` keyword allows you to declare constants, whose values cannot be re-assigned or re-declared.

```javascript
const PI = 3.14;
console.log(PI); // Output: 3.14
PI = 3.14159; // Error: Assignment to constant variable
```

### 2. Arrow Functions

Arrow functions provide a concise syntax for writing function expressions.

```javascript
// Regular function
function add(a, b) {
  return a + b;
}

// Arrow function
const add = (a, b) => a + b;
```

```javascript
// Single parameter, implicit return
const greet = (name) => `Hello, ${name}!`;

// Multiple parameters, explicit return
const add = (a, b) => {
  return a + b;
};

// No parameters, implicit return
const getTime = () => new Date().toLocaleTimeString();

// Object literal with arrow function as method
const person = {
  name: "Alice",
  greet: () => {
    console.log(`Hello, my name is ${this.name}.`); // 'this' refers to the global object, not the 'person' object
  },
};

// Array iteration with arrow function
const numbers = [1, 2, 3, 4, 5];
const doubledNumbers = numbers.map((num) => num * 2);

console.log(greet("John")); // Output: Hello, John!
console.log(add(5, 3)); // Output: 8
console.log(getTime()); // Output: Current time
console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]
person.greet(); // Output: Hello, my name is undefined.
```

### 3. Template Literals

Template literals allow embedded expressions and multi-line strings.

```javascript
const name = "Alice";
const greeting = `Hello, ${name}!
How are you today?`;
console.log(greeting); // output : Hello, Alice! How are you today?
```

### 4. Destructuring Assignment

Destructuring assignment allows you to extract values from objects or arrays into variables.

```javascript
const person = { name: "John", age: 30 };
const { name, age } = person;
console.log(name); // Output: John
console.log(age); // Output: 30
```

### 5. Spread and Rest Operators

Spread and rest operators provide a convenient way to work with arrays and function arguments.

```javascript
// Spread operator
const numbers = [1, 2, 3];
const newNumbers = [...numbers, 4, 5];
console.log(newNumbers); // Output: [1, 2, 3, 4, 5]

// Rest operator
function sum(...args) {
  return args.reduce((total, num) => total + num, 0);
}
console.log(sum(1, 2, 3, 4, 5)); // Output: 15
```

### 6. Modules

Modules allow you to split your code into multiple files and import/export functionality between them.

```javascript
// math.js
export const add = (a, b) => a + b;
export const subtract = (a, b) => a - b;

// app.js
import { add, subtract } from "./math.js";
console.log(add(5, 3)); // Output: 8
console.log(subtract(5, 3)); // Output: 2
```
