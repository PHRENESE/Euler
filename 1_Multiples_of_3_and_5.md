https://projecteuler.net/problem=1

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.
Find the sum of all the multiples of 3 or 5 below 1000.


```javascript
function sumAll(num){
  var natNums = [];
  for(i=1;i<num;i++){
    if(i % 3 === 0 || i % 5 === 0){
      natNums.push(i);
    }      
  }
  var sum = natNums.reduce(function(a, b){
    return a + b;
  });
  console.log(sum);
}

sumAll(1000);
```
