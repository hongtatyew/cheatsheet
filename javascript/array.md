# Array

## Static properties
```js
//  Creates an Array from a String, output: ["🍎", "🍌", "🍇"]
Array.from('🍎🍌🍇'); 
```
```js
// check for an array, output : true
Array.isArray(['🍎', '🍌', '🍇']); 
```
```js
// creates a new Array with provided elements output:["🍎", "🍌", "🍇"]
Array.of('🍎', '🍌', '🍇'); 
```

## Instance properties

```js
// Joins Two arrays, Output : ["🍎", "🍌", "🍇", "🥭"]  
['🍎', '🍌'].concat(['🍇', '🥭']); 
```
```js
//copy first 2 array elements to last 2, output: ["🍎", "🍌", "🍎","🍌"]
['🍎', '🍌', '🍇', '🥭'].copyWithin(2, 0); 
```
```js
// Returns the array that matches our test output : ["🍎"] 
['🍎', '🍌', '🍇'].filter(emoji => emoji === '🍎'); 
```
```js
// fill all the array elements with "🍑", output ['🍎','🍑','🍑','🍒']
['🍎','🍌','🍇','🍒'].fill('🍑',2,3) 
```
```js
// element in the array that has a value of "🍎", output : "🍎"
['🍎', '🍌', '🍇'].find(emoji => emoji === '🍎'); 
```
```js
// get the index of  🍌, output: 1 
['🍎', '🍌', '🍇'].indexOf('🍌'); 
```
```js
// returns the index of the first element  that satisfies the provided testing function. 🍌, output: 1
['🍎', '🍌', '🍇'].findIndex(emoji => emoji === '🍌'); 
```
```js
// executes a provided function once for each array element, output :🍎🍌🍇 
['🍎', '🍌', '🍇'].forEach(emoji => console.log(emoji)); 
```
```js
// Creates a new array by replacing with the return of a function for each array element, output: [🍎🍒, 🍌🍒 , 🍇🍒]
['🍎', '🍌', '🍇'].map(emoji => emoji + '🍒'); 
```
```js
// Check if every element in the array has a value 🍎, Output : false 
['🍎', '🍌', '🍇'].every(emoji => emoji === '🍎'); 
```
```js
// Check if atleast one element in the array has a value 🍎, Output : true 
['🍎', '🍌', '🍇'].some(emoji => emoji === '🍎'); 
```
```js
// Check if the fruit array contains "🥭", output : false 
['🍎', '🍌', '🍇'].includes('🥭'); 
```
```js
// Joins all elements of an array into a string, output : "🍎 + 🍌 + 🍇"
['🍎', '🍌', '🍇'].join(' + '); 
```
```js
// Removes and return the last element of an array, output: "🍇" 
['🍎', '🍌', '🍇'].pop(); 
```
```js
// Adds new elements to the end of an array and returns length, output: 4 
['🍎', '🍌', '🍇'].push('🍒'); 
```
```js
// Reverses the order of the elements in an array, output: ["🍇", "🍌", "🍎"] 
['🍎', '🍌', '🍇'].reverse(); 
```
```js
// Adds/Removes elements output: (removed array) ["🍌", "🍇"]  (new array) ["🍎"] 
['🍎', '🍌', '🍇'].splice(1, 2); 
```
```js
// Selects a part of an array, and returns the new array, output: ["🍌"] 
['🍎', '🍌', '🍇'].slice(1, 2); 
```
```js
// Converts an array to a string, and returns the result, output:"🍎,🍌,🍇" 
['🍎', '🍌', '🍇'].toString(); 
```
```js
// Removes the first element of an array, and returns that element, output: "🍎" 
['🍎', '🍌', '🍇'].shift(); 
```
```js
// Adds new elements to the beginning and returns the new length, output: 4 
['🍎', '🍌', '🍇'].unshift('🍐'); 
```
```js
// Reduce the values of an array to a single value, output: "🍒🍎🍌🍇"
['🍎', '🍌', '🍇'].reduce((acc, cur) => acc + cur, '🍒'); 
```
