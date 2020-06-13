# Create a function that takes three parameters and returns an array with the first parameter x, the second parameter y, and every number in between the first and second parameter in ascending order. Then filter through the array and return the array with numbers that are only divisible by the third parameter n.

Examples

arrayOperation(1, 10, 3) ➞ [3, 6, 9]

arrayOperation(7, 9, 2) ➞ [8]

arrayOperation(15, 20, 7) ➞ []

Notes

The final array should consist of all numbers between x and y inclusive that are divisible by n.
Return an empty array if there are no numbers that are divisible by n.

```javascript
function arrayOperation(x, y, n) {
  let arr = [];
  for (let i = x; i <= y; i++) {
    arr.push(i);
  }
  return arr.filter((x) => x % n === 0);
}
```
