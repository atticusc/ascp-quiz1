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
  4. reduce
  Why reduce? It's great when you want to reduce the values in an array to a single value
  ```javascript
  var ageSum=ages.reduce((total,age=> total +age,0);
  console.log(ageSum)l
  ```
  5. some 
  Why some? It's great method to test whether at least one element in the array passes the test implemented by the provided function
  ```javascript
  [2, 5, 8, 1, 4].some(x => x > 10);  // false
[12, 5, 8, 1, 4].some(x => x > 10); // true
  ```
  
  6. sort
  Why sort? It's the thing to use if you want to put the values of an array in a different order
  ```javascript
  var sortedCompanies=companies.sort((c1,c2)=>
  (c1.start?c2.start?1:-1));
  ```

## Other Important Methods

1. push
`myArr.push("e");` -->// pushes "e" onto the array, and it returns the length. It would return //-> 8
