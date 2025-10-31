# **Modifying Elements at Specific Positions:** _splice()_ and _slice()_

### Retrieving segment of array with _slice()_ method

copies part of array, creates new array

takes 2 args:

-index where new array begins

-index where it ends, excluding that element

(same as with slicing strings, array is sliced at indices provided in args, and new array includes elements between the 2 slices)

```js
const months = [
  "January",
  "February",
  "March",
  "April",
  "May",
  "June",
  "July",
  "August",
  "September",
  "October",
  "November",
  "December",
];

// starting from the element with an index of 2 ("March") to the element with an index of 5, but not including it ("June")
const spring = months.slice(2, 5);

console.log(spring); // ["March", "April", "May"]

console.log(
  months
); /* ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"] */

// As you can see, the original array is the same as before
```

if second arg ommitted, returns all elements after first slice:

```js
const months = [
  "January",
  "February",
  "March",
  "April",
  "May",
  "June",
  "July",
  "August",
  "September",
  "October",
  "November",
  "December",
];

// select all elements starting from index 9 through the end of the array
const fourthQuarter = months.slice(9);
fourthQuarter; // ["October", "November", "December"]
```

if negative numbers passed, counts backwards from end of array:

```js
const months = [
  "January",
  "February",
  "March",
  "April",
  "May",
  "June",
  "July",
  "August",
  "September",
  "October",
  "November",
  "December",
];

// starting from the fourth element from the end to the first element from the end, but not including it
const autumn = months.slice(-4, -1);
console.log(autumn); // ["September", "October", "November"]

// from the third element from the end through the end of the array
const fourthQuarter = months.slice(-3);
console.log(fourthQuarter); // ["October", "November", "December"]
```

if no args, returns new array with all elements of original:

```js
const months = [
  "January",
  "February",
  "March",
  "April",
  "May",
  "June",
  "July",
  "August",
  "September",
  "October",
  "November",
  "December",
];

const monthsCopy = months.slice();

console.log(monthsCopy);

/*
[
    "January",
    "February",
    "March",
    "April",
    "May",
    "June",
    "July",
    "August",
    "September",
    "October",
    "November",
    "December"
  ]
*/
```
