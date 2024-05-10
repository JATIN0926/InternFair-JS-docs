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

#### Explanation:

- The backticks (\`) are used to create template literals in JavaScript.
- Inside a template literal, you can embed expressions using `${}` syntax.
- When JavaScript encounters `${}`, it evaluates the expression inside the curly braces and includes the result in the string.

### JavaScript Variables and Data Types

Variables are used to store data values in JavaScript. JavaScript supports various data types, each serving different purposes. Majorly data types are :

- **Numbers**
- **Strings**
- **Booleans**
- **Arrays**
- **Objects**

Let's explore the different data types and their key points:

**Numbers**

JavaScript represents numbers using the number data type. Numbers can be integers , floating-point numbers or negative numbers.

```javascript
let age = 25;
let pi = 3.14;
```

**Strings**

Strings are sequences of characters enclosed within single quotes ('') or double quotes (""). Strings are immutable(cannot be modified once declared).

```javascript
let name = "Alice";
let message = "Hello, world!";
```

**Booleans**

Booleans represent logical values: true or false. They are commonly used in conditional statements and logical expressions.

```javascript
let isStudent = true;
let isValid = false;
```

**Arrays**

Arrays are ordered collections of values, each identified by an index. They can contain elements of different data types.

```javascript
let numbers = [1, 2, 3, false, "yellow"];
let colors = ["red", "green", "blue", true];
```

**Objects**

Objects are collections of key-value pairs, where keys are strings and values can be any data type.

```javascript
let person = { name: "John", age: 30 };
let book = { title: "JavaScript Basics", pages: 100 };
```

## Accessing Object Properties

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

### Understanding Variable Scope in JavaScript

---

### **let**, **var**, and **const**

**let**

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

**var**

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

**const**

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

### Operators

Operators in JavaScript are symbols or keywords that perform operations on operands (variables or values). They are used to perform arithmetic, comparison, logical, and assignment operations

**Arithmetic Operators**

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

**Comparison Operators**

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

# Explanation of Outputs

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

### Comments

Comments are used to add explanatory notes to JavaScript code. JavaScript supports both single-line and multi-line comments.

```javascript
// This is a single-line comment

/*
This is a
multi-line comment
*/
```

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

### Conditional Statements (if-else, switch):

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

### Loops (for, while, do-while):

Loops are fundamental in programming as they allow us to execute a block of code repeatedly. JavaScript provides several types of loops, each with its own unique characteristics and use cases

**for Loop**

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

**while Loop**

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

**do-while Loop**

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

### Break and Continue Statements

`break` and `continue` statements are used to control the flow of loops. These are also called _Jump_ Statements

**break Statement**

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

### JavaScript Functions

Functions are reusable blocks of code that perform a specific task or calculate a value. They allow for modular programming and help in organizing code for better readability and maintainability.

**What are Functions?**

A function is a block of code that performs a specific task or calculates a value. It consists of a set of statements that are executed when the function is called. Functions can take inputs, known as parameters, and can optionally return a value.

**Declaring Functions**

A function in JavaScript can be declared using the `function` keyword followed by the function name, parentheses `()`, and curly braces `{}` to define the function body.

```javascript
function greet() {
  console.log("Hello, world!");
}
```

**Calling Functions**

To execute a function and perform its task, you need to call it by using its name followed by parentheses `()`.

```javascript
greet(); // Output: Hello, world!
```

**Function Parameters**

Functions can accept inputs, called parameters, which are specified within the parentheses `()`. These parameters allow functions to perform tasks with different values.

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}

greet("Alice"); // Output: Hello, Alice!
```

**Return Statement**

A function can optionally return a value using the `return` statement. This allows the function to provide a result that can be used elsewhere in the code.

```javascript
function add(a, b) {
  return a + b;
}

let result = add(3, 5);
console.log(result); // Output: 8
```

**Anonymous Functions**

Anonymous functions, also known as function expressions, are functions without a name. They are often used as arguments to other functions or assigned to variables.

```javascript
let greet = function () {
  console.log("Hello, world!");
}; // Anonymous function on R.H.S

greet(); // Output: Hello, world!
```

**Arrow Functions**

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

### Exercise Time!

## Exercise Time!

# Exercise Time!

_Note:_ Challenge yourself by attempting to solve these questions on your own before peeking at the answers! It's a great way to test your understanding and strengthen your problem-solving skills

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
