Sure! Here are the condensed code snippets for the important terms and ideas mentioned:

1. Using `find` to find the first element greater than a specified value:
```javascript
const scores = [70, 85, 93, 79, 88];
const passingScore = scores.find(score => score > 75);
```

2. Using `find` to find the first even score in an array:
```javascript
const scores = [77, 82, 91, 88, 95];
const firstEven = scores.find(score => score % 2 === 0);
```

3. Using `findIndex` to find the index of the first element greater than a specified value:
```javascript
const scores = [70, 85, 93, 79, 88];
const passingScoreIndex = scores.findIndex(score => score > 75);
```

4. Using `findIndex` to find the index of the first even score in an array:
```javascript
const scores = [77, 82, 91, 88, 95];
const firstEvenIndex = scores.findIndex(score => score % 2 === 0);
```

5. Creating a custom partition function using `findIndex`:
```javascript
function partition(array, pivot) {
  const pivotIndex = array.findIndex(element => element > pivot);
  const left = array.slice(0, pivotIndex);
  const right = array.slice(pivotIndex);
  return [left, right];
}

const scores = [0, 0, 0, 75, 77, 80, 85, 88, 93];
const result = partition(scores, 75);
```

These code snippets demonstrate the usage of `find` and `findIndex` in various scenarios. The first two snippets use `find` to find specific elements in an array based on conditions. The next two snippets use `findIndex` to find the index of specific elements. The last snippet shows how `findIndex` can be used to create a custom partition function that splits an array into two sub-arrays based on a pivot point.