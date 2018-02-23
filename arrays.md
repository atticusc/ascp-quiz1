# Arrays

## Declaring and Assigning values 
```javascript
var a; //Declaring value

a = [1,2,3]; //Assinging value
```


## Array looping methods

  1. forEach
```javascript
var array1 = ['a', 'b', 'c'];

array1.forEach(function(element) {
  console.log(element);
});

// expected output: "a"
// expected output: "b"
// expected output: "c"
```
  2. map
  ```javascript
  var array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]

  ```
  3. filter
  ```javascript
var words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]

  ```
  4. reduce
  ```javascript
  const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// expected output: 10

// 5 + 1 + 2 + 3 + 4
console.log(array1.reduce(reducer, 5));
// expected output: 15

  ```
  5. some 
  ```javascript
  var array = [1, 2, 3, 4, 5];

var even = function(element) {
  // checks whether an element is even
  return element % 2 === 0;
};

console.log(array.some(even));
// expected output: true

  ```

## Other Important Methods

  1. push `drawXCell()` is a function that draws an XCell to the screen. 
  ```javascript
  for (var x = 1; x < 3; x++){
  
  }
  ```
  2. pop() this method removes the last value from the existing array. 
  ```javascript
  var plants = ['broccoli', 'cauliflower', 'cabbage', 'kale', 'tomato'];

console.log(plants.pop());
// expected output: "tomato"

console.log(plants);
// expected output: Array ["broccoli", "cauliflower", "cabbage", "kale"]

plants.pop();

console.log(plants);
// expected output: Array ["broccoli", "cauliflower", "cabbage"]
  ```
