Terms and Definitions:

1. `map`: An array method that creates a new array by applying a transformation or mapping function to each element of the original array. It executes a callback function on each element and collects the return values in a new array, preserving the order of the elements.
   - Syntax: `array.map(callback(element[, index[, array]])[, thisArg])`
   - Example:
     ```javascript
     const numbers = [1, 2, 3];
     const doubledNumbers = numbers.map(number => number * 2);
     console.log(doubledNumbers); // [2, 4, 6]
     ```

2. `filter`: An array method that creates a new array with all elements that pass a specific condition (determined by a callback function).
   - Syntax: `array.filter(callback(element[, index[, array]])[, thisArg])`
   - Example:
     ```javascript
     const numbers = [1, 2, 3, 4, 5];
     const evenNumbers = numbers.filter(number => number % 2 === 0);
     ```

3. Callback function: A function that is passed as an argument to another function and is called within that function. In the context of array methods like `map` and `filter`, the callback function is applied to each element of the array and determines the transformation or filtering condition.

4. Function declaration: A way to define a function using the `function` keyword followed by a name, parameters, and a function body.

5. Function expression: A way to define a function by assigning it to a variable. The function is created without a name and can be assigned and passed around like any other value.

6. Anonymous function: A function that is defined without a specific name and can be used directly as a callback function or assigned to a variable.

7. Chaining methods: The practice of applying multiple array methods sequentially by calling them one after another on an array, which allows for complex operations to be performed in a concise and readable manner.

By understanding the concepts of `map`, `filter`, callbacks, function declaration, function expression, anonymous functions, and chaining methods, you can leverage the power of JavaScript to manipulate and transform arrays efficiently.