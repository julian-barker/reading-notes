[Home](../README.md)

# Class 03

## Lists and Keys

1. The `.map()` method returns a an array of equal length as the array we call the method on
2. If you want to display each item in an array in JSX, you can use the .map method to iterate throught the array and return a component or element containing the value at each index of the array.
3. Each list item needs a unique key prop.
4. The purpose of the key is for React to keep track of the different sibling components

## Spread Operator

1. The spread operator (`...`) is an operator used to deconstruct an array into a list of its contents
2. It is useful for:

    - copying an array
    - combining arrays
    - math functions (such as Math.min())
    - using an array as arguments
    - adding an item to a list
    - adding to state in React
    - combining objects
    - converting NodeList to an array

3. `[...arr1, ...arr2]` - combines two arrays (`arr1` and `arr2`)
4. `[...arr, newItem]` - adds a new item (`newItem`) to an array (`arr`)
5. `[...obj1, ...obj2, newKV]` - combines two objects (`obj1` and `obj2`) and adds a new entry (`newKV`)

## Passing Functions

1. The first step of passing functions between objects is to create the function and pass it into the child props
2. The `increment` function updates the state by creating and returning a new Array of person objects, incrementing the count on whichever person object matches the name passed in as an argument.
3. You can pass a method from parent to child by including it in the child's props
4. The child component invokes a method passed down either through an eventlistener, or by calling that function from its props in one of its methods
