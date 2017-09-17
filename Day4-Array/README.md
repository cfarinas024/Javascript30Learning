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
* array functions (filter, map, sort, reduce,)
