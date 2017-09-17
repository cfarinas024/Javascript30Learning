# Array functions

Javascript array functions

## Concepts learned:
* refactoring if statements with:
Arrow functions:
```sh
const fullNames = inventors.map(function(inventor) {
  return inventor.first + ' ' + inventor.last
});
```
```sh
const fullNames = inventors.map(inventor => inventor .first + ' ' + inventor.last)
```
Back ticks:
```sh
const fullNames = inventors.map(inventor => `${inventor.first} ${inventor.last}`)
```
Ternary Expressions:
```sh
const ordered = inventors.sort(function(a, b) {
  if(a.year > b.year) {
    return 1;
  } else {
    return -1;
  }
})
```
```sh
const ordered = inventors.sort((a,b) => a.year > b.year ? 1 : -1);
```
Reduce method
```sh
var totalYears = 0;

for(var i = 0; i < inventors.length; i++) {
  totalYears += inventors[i].year
}
```
```sh
const totalYears = inventors.reduce((total, inventor) => {
  return total + (inventor.year);
}, 0)
```
* Creating array from querySelectorAll
```sh
const links = Array.from(category.querySelectorAll('.mw-catogory a'))
```
or
```sh
const links = [...category.querySelectorAll('.mw-category a')]
```
