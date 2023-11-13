# daily-coding-tips
#### This is a curation of coding tips I do share daily starting from November 6, 2023

```javascript
// Create a sequence of numbers in 1 line of code
Array.from({ length: n }, (_, i) => i)
// Or
[...Array(n).keys()]

Array.from({ length: 12 }, (_, i) => i+1) // This sequence will start from 1

// Example
Array.from({ length: 10 }, (_, i) => i+1) // outputs : [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```
###### Remove all falsy values from an array <!--Nov 9 -->
```javascript
// in 1 line of code, remove all falsy values from an arr
array.filter(Boolean);

// Example
[false, 0, true, 2, '', 'aroyehun'].filter(Boolean)
// outputs: [ true, 2, 'aroyehun' ]
```

* Format a Number as a currency
```javascript
const formatCurrency = (number, currency = 'USD') => new Intl.NumberFormat('en-US', { style: 'currency', currency }).format(number);
```

* Capitalize The First Character of Each Word in a String
```javascript
const Capitalize = (str) => str.replace('/\b\w/g', char => char.toUpperCase())

// Example
Capitalize('i am a slave of Allah') // 'I Am A Slave Of Allah'
```
// Nov 13, 2023
* Identify the shared items between two arrays
```javascript
const arrayIntersection = (arr1, arr2) => arr1.filter(item => arr2.includes(item));

// Example
arrayIntersection(['aroyehun', 2, 3, 4], ['ahmad', 20, 2, 4]) // [2, 4]
```
