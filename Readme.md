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

- **Equal (==):** Checks if two operands are equal.
- **Not Equal (!=):** Checks if two operands are not equal.
- **Strict Equal (===):** Checks if two operands are equal and of the same type.
- **Strict Not Equal (!==):** Checks if two operands are not equal and/or not of the same type.
- **Greater Than (>):** Checks if the left operand is greater than the right.
- **Less Than (<):** Checks if the left operand is less than the right.
- **Greater Than or Equal (>=):** Checks if the left operand is greater than or equal to the right.
- **Less Than or Equal (<=)::** Checks if the left operand is less than or equal to the right.

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
