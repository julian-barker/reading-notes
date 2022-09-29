[Home](../README.md)

# Class 09

## Functional Programming

1. What is functional programming?
  Functional programming is a programming paradigm wherein computation is simply the evaluation of mathematical functions and data and state are not mutated.

2. What is a pure function and how do we know if something is a pure function?
  A pure function should not rely on any data other than those passed in as arguments, and should return new values, rather than changing exixsting values declared outside the scope of the function (called side-effects).

3. What are the benefits of a pure function?
  Pure functions increase predicatability and reduce the chance for unexpected errors.

4. What is immutability?
  Immutability refers to a piece of data not changing over time. The state of a variable will always remain the same.

5. What is Referential transparency?
  Referential transparency refers to always producing the same outputs for the same inputs. It is the combination of pure functions and immutable data.

# Node JS - modules and require

1. What is a module?
  A module is a piece of code separated into a different file that will be imported into another file.

2. What does the word ‘require’ do?
  Require conditionally brings in a module from somewhere else and assigns it to a variable.

3. How do we bring another module into the file the we are working in?
  We use `import` or `require` statements. `import` is ES6 language.

4. What do we have to do to make a module available?
  In order to make the module available, we have to export specific functions in that module for use in other files.
