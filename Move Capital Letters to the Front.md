# Create a function that moves all capital letters to the front of a word.

Examples

capToFront("hApPy") ➞ "APhpy"

capToFront("moveMENT") ➞ "MENTmove"

capToFront("shOrtCAKE") ➞ "OCAKEshrt"

Notes

Keep the original relative order of the upper and lower case letters the same.

```javascript
function capToFront(s) {
  return s.match(/[A-Z]/g).join("") + s.match(/[a-z]/g).join("");
}
```
