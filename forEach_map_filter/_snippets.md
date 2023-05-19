Sure! Here are some code snippets that can help you learn and understand the concepts discussed in the transcript:

1. Custom `map` implementation:
```javascript
function myMap(array, callback) {
  const mappedArray = [];
  for (let i = 0; i < array.length; i++) {
    const val = callback(array[i], i, array);
    mappedArray.push(val);
  }
  return mappedArray;
}
```

2. Example usage of `myMap`:
```javascript
const numbers = [1, 2, 3];
const doubledNumbers = myMap(numbers, number => number * 2);
console.log(doubledNumbers); // [2, 4, 6]
```

3. Custom `forEach` implementation:
```javascript
function myForEach(array, callback) {
  for (let i = 0; i < array.length; i++) {
    callback(array[i], i, array);
  }
}
```

4. Example usage of `myForEach`:
```javascript
const colors = ['red', 'green', 'blue'];
myForEach(colors, val => console.log(val.toUpperCase()));
```

5. Custom `filter` implementation:
```javascript
function myFilter(array, callback) {
  const filteredArray = [];
  for (let i = 0; i < array.length; i++) {
    if (callback(array[i], i, array)) {
      filteredArray.push(array[i]);
    }
  }
  return filteredArray;
}
```

6. Example usage of `myFilter`:
```javascript
const numbers = [1, 2, 3, 4, 5];
const evenNumbers = myFilter(numbers, number => number % 2 === 0);
console.log(evenNumbers); // [2, 4]
```

7. Example combining `map` and `filter`:
```javascript
const words = ['apple', 'banana', 'orange'];
const filteredMappedWords = words
  .filter(word => word.length <= 5)
  .map(word => word.toUpperCase());
console.log(filteredMappedWords); // ['APPLE', 'ORANGE']
```

These code snippets demonstrate the implementation and usage of custom `map`, `forEach`, and `filter` functions, as well as examples of combining these array methods. They should help you understand and practice the concepts discussed in the transcript.