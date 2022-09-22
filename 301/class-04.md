[Home](../README.md)

# Class 04

## Forms

1. Controlled components are form elements whose value is controlled by React state
2. It makes more sense to update it in real-time, as this can be useful for things such as fuzzy search. It depends on what you want to do
3. We use `event.target.value` to grab the value of an input element as it is changed.
 
## Ternary Operator

1. The ternary operator is useful to simplify the syntax of code and reduce the number of lines of code. It is most useful when dealing with single if else statements that would return a value in either case, although you can also nest them
2.

``` javascript
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

can be re-written as:

``` javascript
x === y ? console.log(true) : console.log(false);
```
