# Create a function that takes a string and replaces the vowels with another character.

a = 1
e= 2
i = 3
o = 4
u = 5

Examples
replaceVowel("karachi") ➞ "k1r1ch3"

replaceVowel("chembur") ➞ "ch2mb5r"

replaceVowel("khandbari") ➞ "kh1ndb1ri"

Notes
The input will always be in lowercase.

```javascript
const replaceVowel = (word) =>
  word
    .replace(/a/g, 1)
    .replace(/e/g, 2)
    .replace(/i/g, 3)
    .replace(/o/g, 4)
    .replace(/u/g, 5);
```
