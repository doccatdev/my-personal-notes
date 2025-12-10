# Javascript

## Javascript Basics

### Data Type (Primitive)

- String

```javascript
let name = "John Doe";
console.log(name); // John Doe
```

- Number

```javascript
let number = 100;
console.log(number); // 100
```

- Boolean

```javascript
let status = true;
console.log(status); // true
```

```javascript
let status = false;
console.log(status) // false
```

- Null

```javascript
let age = null;
console.log(age); // null
```

- Undefined

```javascript
let b;
console.log(b); // undefined
```

- Symbol

```javascript
let s1 = Symbol("Hello");
let s2 = Symbol("Hello");
console.log(s1 == s2); // false
```

- BigInt

```javascript

```

!!! info "Javascrip NaN"

- NaN stands for "Not a Number" and represents an undefined or unrepresentable value in JavaScript.
- Despite its name, NaN is considered a number type in JavaScript.
- Operations involving NaN generally result in NaN.
- NaN often appears when performing invalid mathematical operations or when input is not a valid number.

```javascript
let num1 = 0;
let num2 = 0;
console.log(num1 / num2) // NaN
```

### Variable & Let

!!! note "Key Takeaways"

- Variables in JavaScript allow us to store values with names for later use or updates.
- The `let` keyword is used to declare variables that can be reassigned.
- Variables hold snapshots of values; updating one variable does not automatically update others dependent on it.
- Proper variable naming and understanding of variable behavior are essential for effective coding.

```javascript
let x = 5;
console.log(x); // 5
```

### Shorthand Operator and Increment/Decrement

#### Shorthand Operator

- `+=`

```javascript
let score = 5;
// score = score + 5
score += 5; 
console.log(score); // 10
```

- `-=`

```javascript
let score = 5;
// score = score - 5
score -= 5; // 0
console.log(score);
```

- `*=`

```javascript
let score = 5;
// score = score * 5
score *= 5; 
console.log(score); // 25
```

- `/=`

```javascript
let score = 5;
// score = score / 5
score /= 5; 
console.log(score); // 1
```

#### Increment/Decrement

- Increment

```javascript
let score = 5;
// score = score + 1
score++;
console.log(score); // 6
```

- Decrement

```javascript
let score = 5;
// score = score - 1
score--;
console.log(score); // 4
```

!!! info "`i++` vs `++i`"

- i++ is the post-increment operator that returns the value before incrementing.
- ++i is the pre-increment operator that increments the value first and then returns it.

### Operator

- To perform specific action on value or variables

#### Arithmetic Operator

##### Addition

```javascript
let num_1 = 3;
let num_2 = 4;
console.log(num_1 + num_2); // 7
```

##### Subtraction

```javascript
let num_1 = 15;
let num_2 = 4;
console.log(num_1 - num_2); // 11
```

##### Multiplication

```javascript
let num_1 = 15;
let num_2 = 4;
console.log(num_1 * num_2); // 60
```

##### Division

```javascript
let num_1 = 15;
let num_2 = 4;
console.log(num_1 / num_2); // 3.75
```

##### Modulo

```javascript
let num_1 = 15;
let num_2 = 4;
console.log(num_1 % num_2); // 3
```

##### Exponent (Power of numbers)

```javascript
let num_1 = 2;
let num_2 = 4;
console.log(num_1 ** num_2); // 16
```

#### Comparison Operator

- To compare two value

```javascript
let number = 7;
console.log(number < 8); // true

let number = 7;
console.log(number > 8); // false

let number = 7;
console.log(number == 8); // false

let number = 7;
console.log(number <= 8); // true

let number = 7;
console.log(number >= 8); // false

let number = 7;
console.log(number != 8); // true
```

### Var and Const

!!! note "Key Takeaways"

- The `const` keyword creates variables whose values cannot be changed after assignment.
- Use `const` for values that are meant to remain constant, such as mathematical constants or conversion factors.
- The `var` keyword is the old way of declaring variables in JavaScript, but `let` and `const` are now preferred.
- Use `let` for variables that need to be reassigned, and avoid using `var` in modern JavaScript code



- Const

```javascript
const pi = 3.14;
consloe.log(pi); // 3.14
```

### Variable Naming Rules

!!! info "Variable Naming Rules"

- Start with a letter
- Be consistent with the style
- If the variable have more that words, use camel case
- Choose descriptive and meaningful name

## JavaScript String and More

### String

!!! note "Key Takeaways"

- String is another primitive data type in JavaScript 
- Represent text and must be wrapped in quotes

```javascript
// double quote

let username = "John Doe";
console.log(username); // John Doe

// single quotes: 

let firstName = "John";
console.log(firstName); // John
```

### Indices & Length

!!! note "Key Takeaways"

- Strings in JavaScript are indexed collections where each character has a positional number starting from zero
- Individual characters in a string can be accessed using square brackets with the index number
- The `.length` property of a string returns the total number of characters, which is always one more than the highest index
- Strings are immutable; you cannot change a character directly but can create new strings through concatenation or reassignment

#### Indices

```javascript
let animals = "Dumbo Octopus";
console.log(animals); // Dumbo Octopus

// accessing through index

console.log(animals[0]); // D
console.log(animals[5]); // Blank space
console.log(animals[12]); // s
```

#### Length

```javascript
let animals = "Dumbo Octopus";
console.log(animals); // Dumbo Octopus
console.log(animals.length); // 13
```

!!! info "String Concatenate"

- Joining two or more string together to form a single new string

```javascript
let firstName = "John";
let lastName = "Doe";
console.log(firstName + lastName); // JohnDoe
```

### String Methods

!!! note "Key Takeaways"

- Methods is build-in function that can help perform action with individual strings

- `.toUpperCase()` : Make all string text uppercase

```javascript
let message = "leave me alone right now! i hate you";
console.log(message.toUpperCase()); // LEAVE ME ALONE RIGHT NOW! I HATE YOU
```

- `.toLowerCase()` : Make all string text lowercase

```javascript
let message = "AAAAAAAAAAA RUN RUN RUN";
console.log(message.toLowerCase()); // aaaaaaaaaaa run run run
```

- `.trim()` : Remove whitespaces from both ends (leading and trailing)

```javascript
let message = "                leave me alone                    ";
console.log(message.trim()); // leave me alone (without spacing)
```

#### String Methods with Arguments

!!! note "Key Takeaways"

- Some method accepted to pass argument from build in functions

- `.indexOf()`: find the first occurrence of a specified value within a string or an array. It returns the index (position) of the first instance found, or -1 if the value is not present

```javascript
let messageOne = "hahaha that is so funny"
console.log(messageOne.indexOf('y')); // 22

// if the value is not presented
let message = "hahaha that funny"
console.log(message.indexOf('z')); // -1
```

- `.slice()` : extracts or slices a portion of a string and returns it as a new string.

```javascript
let messageOne = "hahaha that is so funny"
console.log(messageOne.slice(6)); // that is so funny

let messageTwo = "hahaha that is so funny"
console.log(messageTwo.slice(6,15)); // that is 

// start from backwards

let messageThree = "hahaha that is so funny"
console.log(messageThree.slice(-1)); // that is 
```

- `.replace()` : replace parts of a string

```javascript
let messageThree = "hahaha that is so funny"
console.log(messageThree.replace("hahaha", "lolololololol")); // lolololololol that is so funny
```

- `.repeat()` :  returns a new string which contains the specified number of copies of this string, concatenated together

```javascript
let messageThree = "hahaha"
console.log(messageThree.repeat(5)); // hahahahahahahahahahahahahahaha
```

#### String Template Literal

#### Undefined & Null

#### Random Number & Math Object