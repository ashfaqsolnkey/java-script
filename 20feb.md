###1. Find max number from array 
```
let arr =[12,1,23,40,30];
 let max = arr[0];
 for(let i = 0;i < arr.length; i++){
    if(max < arr[i]){
        max=arr[i]
    }
 }
console.log(max)
```


2. find min number from array 

*let arr =[5,10,23,2,40,1,30,4]
let min = arr[0]
 for(let i = 0; i < arr.length;i++){
    if(min > arr[i]){
        min = arr[i]
    }
 }
 console.log(min)*


3. Find total duplicate count of a number 

*let arr = [53, 32,32,32, 64, 53, 43];
let count = 0;
for (let i = 0; i < arr.length; i++) {
    if (arr[i] === 32) {
        count += 1
    }
}
console.log(count)*


4. find middle element of the array 

*function func(){ 
    const arr = [1, 3, 7, 10, 70, 18, 33, 45, 99,20,10]; 
   function mid(arr, i){ 
      while(arr[i]){ 
         return mid(arr, ++i); 
      }; 
      return i % 2 !== 0 ? [arr[(i-1) / 2]] : [arr[(i/2)-1], arr[i/2]]; 
   }
   console.log(mid(arr, i = 0))
}
func()*


5. find last element of the array 

const arr =[2,4,6,7,8]
console.log(arr[arr.length-1])

6. find first element of the array 

const arr =[2,4,6,7,8]
console.log(arr[0])



8. Find total count of odd numbers in array 

const numbers = [8, 19, 5, 6, 14, 9, 13];
const odds = [];
for (const num of numbers) {
  if (num % 2 === 1) {
    odds.push(num);
  }
}
console.log(odds)



9. Find total count of even numbers in array 

const numbers = [8, 19, 5, 6, 14, 9, 13];
const odds = [];
for (const num of numbers) {
  if (num % 2 === 0) {
    odds.push(num);
  }
}
console.log(odds)



 let arr =[12,1,239,40,30]
 let secondHight = arr[0]

 for(let i = 0;i < arr.length; i++){
    if(secondHight < arr[i]){
        secondHight=arr[i]
    }
 }
console.log(secondHight)



10. Find second highest number from array 

const arr = [
    4,
    2,
    3,
    22,
    56,
    90,
    32,
    550,
    2,
    60,
    45,
    220,
    32,
    22,
    2,
    ,
    67,
    43,
    11,
    78,
    2,
    110,
    43,
    21,
    32,
  ];
  let max = arr[0];
  let secondMax = -1;
  for (let i = 0; i < arr.length; i++) {
    if (max < arr[i]) {
      let temp = max;
      max = arr[i];
      secondMax = temp;
    } else if (secondMax < arr[i] && arr[i] < max) {
      secondMax = arr[i];
    }
  }
  console.log(max, secondMax);


11. find second lowest number from array 

const arr = [
    5, 2, 3, 22, 56, 90, 32, 550, 2, 60, 45, 220, 32, 22, 2, 67, 43, 11, 78, 2,
    110, 43, 21, 32, 0,
  ];
  let min = arr[0];
  let secondMin = -1;
  for (let i = 0; i < arr.length; i++) {
    if (min > arr[i]) {
      let temp = min;
      min = arr[i];
      secondMin = temp;
    } else if (secondMin > arr[i] && arr[i] > min) {
      secondMin = arr[i];
    }
  }
  console.log(secondMin, min);



12. Find average of the array 

const arr = [
    5, 2, 3, 22, 56, 90, 32, 550, 2, 60, 45, 220, 32, 22, 2, 67, 43, 11, 78, 2,
    110, 43, 21, 32, 0,
  ];
  let sum = 0;
  for (let i = 0; i < arr.length; i++) {
    sum = sum + arr[i];
  }
  console.log(sum, arr.length, sum / arr.length);


13. Find which number is repeated most number of the times in the array, also tell number along with count

``const arr = [
    5, 2, 3, 22, 56, 90, 32, 550, 2, 60, 45, 220, 32, 22, 2, 67, 43, 11, 78, 2,
    110, 43, 21, 32, 0,
  ];
  const newArr = [];
  for (let i = 0; i < arr.length; i++) {
    if (newArr[arr[i]]) {
      newArr[arr[i]] = newArr[arr[i]] + 1;
    } else {
      newArr[arr[i]] = 1;
    }
  }
  console.log(newArr[110]);``
