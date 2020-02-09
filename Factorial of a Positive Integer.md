# Factorial of a Positive Integer

Examples

factorial(4) ➞ 24

factorial(0) ➞ 1

factorial(9) ➞ 362880

Notes

The factorial of 0 is 1.
The factorial of any positive integer Z is Z _ (Z - 1) _ (Z - 2) _ . . . . . . _ 1 (e.g. factorial of 3 is 3 _ 2 _ 1 = 6).

```javascript
const factorial = num => (num <= 1 ? 1 : num * factorial(num - 1));
```
