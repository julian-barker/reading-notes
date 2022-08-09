[Home](README.md)

# Reading Assignment 8

## Operators and Loops

### Operators

- Arithmetic operators include:
    - `+` addition
    - `-` subtraction
    - `*` multiplication
    - `/` division
    - `**` exponentiation
    - `%` modulus
    - `++` increment
    - `--` decrement

- Assignment operators assign a value to a variable. Examples include:
    - `=` x = y
    - `+=` same as `x = x + y`
    - `-=`, `*=`, `/=`, `**=`, `%=` function in the same pattern as `+=`

- String operators operate on a string or strings. `+` concatenates, and `+=` functions similarly as in arithmetic

- Comparison operators compare two variables and usual return a boolean value (true/false)
    - `==` equal to
    - `===` true equal (equal in value and type)
    - `!=` not equal
    - `>` greater than
    - `<` less than
    - `>=` greater than or equal to
    - `<=` less than or equal to
    - `?` is the ternary operator (aka w.t.f - what-true-false) evaluates an expression and executes one of two expressions based on if the result is truthy or falsy

### Loops

- `for` loops are used to execute an expression a finite number of times
    - the number of iterations can be either based on a predetermined fixed value, or a variable value, such as a counter or length of a string
    - syntax: `for (optional initial value; stop condition; incrementation) {expression to execute}` ex. `for (let i = 0; i < 5; i++) {}`
- `while` loops execute an expression as long as a certain condition remains true. ex. `while(status != complete {})`
- other keywords exist to control loop function, such as `break` or `continue`
