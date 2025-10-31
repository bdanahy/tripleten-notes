# **Adding and Removing Elements:** _shift(), unshift(), push(),_ and _pop()_

### Removing first element with _shift()_ method

_shift()_ removes first element of array, returns removed item

can assign removed item as value of new variable

```js
const italianCities = ["Pompeii", "Rome", "Naples"];

const volcanicEruption = italianCities.shift();

// the shift() method returns the removed element
console.log(volcanicEruption); // "Pompeii"

// now the first element is gone from the array
console.log(italianCities); // ["Rome", "Naples"]
```

if array is initially empty, method returns _undefined_

### Adding an element to beginning of array with _unshift()_ method

can add multiple elements, separated by commas.

array called upon is modified.

```js
const governmentLand = ["National Park Service", "Fish and Wildlife Service", "Forest Service"];

governmentLand.unshift("Department of Defense", "Bureau of Land Management");

console.log(governmentLand);

// ["Department of Defense", "Bureau of Land Management", "National Park Service", "Fish and Wildlife Service", "Forest Service"]
```

changes length of array, returns number of elements

```js
const governmentLand = ["Department of Defense", "Bureau of Land Management", "National Park Service", "Fish and Wildlife Service", "Forest Service"];

console.log(governmentLand.length); // 5
console.log(governmentLand.unshift("Quick question")); // 6
```

_shift()_ and _unshift()_ **change indices of elements!** 

**therefore it is better to use** _pop()_ and _push()_