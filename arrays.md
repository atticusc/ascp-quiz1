# Arrays
Array: a collection of elements; think about it like a bag where you can throw stuff in

## Declaring and Assigning values 

Declarig value: `var myArr;`
Assigning value: `myArr=[1,2,3,4,5,6,7];`
Declaring and Assigning value: `var myArr=[1,2,3,4,5,6,7];`

To get values out of array: `myArr[2];` --> // this returns 3 `myArr[0];` --> //this returns 1

`myArr.length` --> //tells how many items are in the arra7. IT DOESN'T USE ZERO INDEXING

`myArr[myArr.length-1]` --> // index of last item


## Array looping methods

  1. forEach

  Why forEach? It's WAY better for loops
  
 Old:
  ```javascript
  for(var i=o; i<companies.length;i++){
  console.log(companies[i];
  ```
 New: 
 ```javascript
 companies.ForEach(function(company){
 console.log(company.name);
 });
```

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
  Why map? It's great to use when you want to do the same thing to all values in an array. Ex: you could use it if you want to divide every value by two in the array
  
  ```javascript
  var numbers = [1, 4, 9];
var doubles = numbers.map(function(num) {
  return num * 2;
});

// doubles is now [2, 8, 18]
// numbers is still [1, 4, 9]
  ```
  
  ```javascript
  var array1 = [1, 4, 9, 16];

// pass a function to map
const map1 = array1.map(x => x * 2);

console.log(map1);
// expected output: Array [2, 8, 18, 32]

  ```
  
  
  3. filter
  Why filter? It's great to use when you want to get out certain values out of an array
  
  Old:
  ```javascript
  var canDrink =[];
  for(var i=0; i<ages.length; i++){
  if(ages[i] >= 21){
  canDrink.push(ages[i]);
  }
  }
  ```
  New: 
  ```javascript
  
  var canDrink=ages.filter(function(age){
  if(age>=21){
  return true;
  }
  });
  ```
  
  ```javascript
var words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]

  ```
  
  4. reduce
  Why reduce? It's great when you want to reduce the values in an array to a single value
  ```javascript
  var ageSum=ages.reduce((total,age=> total +age,0);
  console.log(ageSum)l
  ```

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
  Why some? It's great method to test whether at least one element in the array passes the test implemented by the provided function
  ```javascript
  [2, 5, 8, 1, 4].some(x => x > 10);  // false
[12, 5, 8, 1, 4].some(x => x > 10); // true
  ```
  
  ```javascript
  var array = [1, 2, 3, 4, 5];

var even = function(element) {
  // checks whether an element is even
  return element % 2 === 0;
};

console.log(array.some(even));
// expected output: true
```
 
  6. sort
  Why sort? It's the thing to use if you want to put the values of an array in a different order
  ```javascript
  var sortedCompanies=companies.sort((c1,c2)=>
  (c1.start?c2.start?1:-1));


## Other Important Methods

  1. push(`...`) is a function that adds new elements to the end of an array. 
  ```javascript
var myArr = [1,2,3] ;
myArr.push(4);
console.log(myArr);
//expected output: [1,2,3,4]

var myArr2 = [[1,2],[3,4]];
myArr2.push([5,6]);
console.log(myArr2);
expected output: [[1,2],[3,4],[5,6]]
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
 3. length gets the length of the array and returns an number
 ```javascript
 var myArr = [0,1,2,3,4,5];
 console.log(myArr.length);
 //expected output: 6
 ```
 
 4. [`...`] gets a spcific element from the array. 
 ```javascript
 var myArr = [0,1,2,3];
 console.log(myArr[0]);
 console.log(myArr[1]);
 console.log(myArr[2]);
 console.log(myArr[3]);
 //expected output: 0
 //expected output: 1
 //expected output: 2
 //expected output: 3
 ```
