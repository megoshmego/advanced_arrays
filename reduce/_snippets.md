Certainly! Here are code snippets that can help you learn and understand the concepts discussed in the provided information:

1. Custom implementation of `reduce`:
```javascript
function myReduce(array, callback, initialValue) {
  let accumulator = initialValue !== undefined ? initialValue : array[0];
  const startIndex = initialValue !== undefined ? 0 : 1;

  for (let i = startIndex; i < array.length; i++) {
    accumulator = callback(accumulator, array[i], i, array);
  }

  return accumulator;
}
```

2. Example usage of `myReduce` to calculate the sum of all elements in an array:
```javascript
const numbers = [1, 2, 3, 4, 5];
const sum = myReduce(numbers, (accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum);
// Output: 15
```

3. Example usage of `myReduce` to find the maximum value in an array:
```javascript
const numbers = [10, 5, 20, 8, 15];
const max = myReduce(numbers, (maxValue, currentValue) => (currentValue > maxValue ? currentValue : maxValue));
console.log(max);
// Output: 20
```

4. Example usage of `myReduce` with an initial value to calculate the product of all elements in an array:
```javascript
const numbers = [1, 2, 3, 4, 5];
const product = myReduce(numbers, (accumulator, currentValue) => accumulator * currentValue, 1);
console.log(product);
// Output: 120
```

5. Example usage of `myReduce` with an object to count occurrences of each element in an array:
```javascript
const fruits = ['apple', 'banana', 'apple', 'orange', 'banana', 'apple'];
const fruitCount = myReduce(
  fruits,
  (count, fruit) => {
    count[fruit] = (count[fruit] || 0) + 1;
    return count;
  },
  {}
);
console.log(fruitCount);
// Output: { apple: 3, banana: 2, orange: 1 }
```

These code snippets demonstrate the implementation and usage of a custom `reduce` function (`myReduce`) as well as examples of using it to perform various operations, such as calculating the sum, finding the maximum value, calculating the product, and counting occurrences. They should help you understand and practice the concepts discussed in the provided information.