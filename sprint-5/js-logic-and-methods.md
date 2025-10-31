# **Merging and Joining Arrays:** _concat() and join()_

### Joining arrays with concat() method

```js
const toDoList = ["Plant tree", "Build house"];
const toDoListUpdated = toDoList.concat(["Raise children"]);

console.log(toDoListUpdated);

// ["Plant tree", "Build house", "Raise children"]
```

arguments don't have to be only arrays:

```js
const classA = ["John", "Emma", "Mia", "Lucas"];
const classB = ["Oliver", "Sophia", "Ava"];
const student = "Frank";

const allStudents = classA.concat(classB, student);

console.log(allStudents);

// ['John', 'Emma', 'Mia', 'Lucas', 'Oliver', 'Sophia', 'Ava', 'Frank']
```

you can pass another array as an argument. elements of array will be copied and added to new array:

```js
const washingtonDCAttractions = ["The Lincoln Memorial", "United States Capitol"];
const newYorkAttractions = ["Metropolitan Museum of Art", "Broadway"];
const sanFranciscoAttractions = ["Golden Gate Bridge", "Chinatown"];

const usaAttractions = washingtonDCAttractions.concat(newYorkAttractions, sanFranciscoAttractions);

// will return a new array containing all the values of the original arrays

console.log(usaAttractions);

/*
  [
    "The Lincoln Memorial",
    "United States Capitol",
    "Metropolitan Museum of Art",
    "Broadway",
    "Golden Gate Bridge",
    "Chinatown"
  ]
*/
```

**The concat() method doesn't change the original array, it returns a new one. Any changes you make to the new array won't affect the original array.**

*******

