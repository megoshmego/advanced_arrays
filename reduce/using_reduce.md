Important terms and ideas:

1. Reduce: A built-in array method in JavaScript that allows us to reduce an array or collection of values down to a single value by applying a callback function to each element.
2. Accumulator: The first parameter of the callback function in `reduce`. It represents the value that is being reduced or accumulated during each iteration.
3. Callback function: A function passed to `reduce` that defines the logic for the reduction. It takes two parameters: the accumulator and the current element being iterated.
4. Optional second parameter: An optional parameter that can be provided to `reduce` as the initial value of the accumulator. If not provided, the first element of the array is used as the initial value.
5. Iteration and updating the accumulator: `reduce` iterates over each element of the array, applying the callback function to each element and updating the accumulator accordingly.
6. Returning a value: The value returned by the callback function becomes the new value of the accumulator for the next iteration.
7. Reducing to different values: The callback function can be used to perform different operations, such as finding the minimum or maximum value, summing all elements, or concatenating strings.
8. Ternary operator: A shorthand conditional operator that can be used in the callback function to write concise conditional statements.
9. Initializing the accumulator: The optional second parameter of `reduce` can be used to initialize the accumulator to a specific value, instead of using the first element of the array.

Code snippets:

1. Summing all elements of an array using `reduce`:
```javascript
const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum);
// Output: 15
```

2. Finding the minimum value in an array using `reduce`:
```javascript
const scores = [88, 93, 79, 85, 91];
const minScore = scores.reduce((min, score) => (score < min ? score : min), scores[0]);
console.log(minScore);
// Output: 79
```

3. Reducing two arrays and finding the minimum overall value:
```javascript
const midtermScores = [88, 93, 94, 64, 62, 56];
const finalScores = [92, 93, 76, 77, 78, 59, 61];

const minOverallScore = finalScores.reduce((min, score) => (score < min ? score : min), midtermScores[0]);
console.log(minOverallScore);
// Output: 56
```

These code snippets demonstrate the usage of `reduce` in various scenarios. The first snippet shows how to sum all the elements of an array, the second snippet finds the minimum value in an array, and the third snippet combines two arrays and finds the minimum overall value using `reduce`.