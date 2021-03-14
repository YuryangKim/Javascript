# 제어문 연습 문제

1. 변수 x가 10보다 크고 20보다 작을 때 변수 x를 출력하는 조건식을 완성하라 


```javascript
  var x = 15;

  if(10 < x < 15){
    console.log(x);
  }
```


2. for문을 사용하여 0부터 10미만의 정수 중에서 짝수만을 작은 수부터 출력하시오.


output


```
0
2
4
6
8
```


Answer


```javascript
for(i = 0; i < 10; i++){
  if(i % 2 == 0) 
    console.log(i);
}
```


3. for문을 사용하여 0부터 10미만의 정수 중에서 짝수만을 작은 수부터 문자열로 출력하시오.


output


```
02468
```


Answer


```javascript
let str = '';
for(i = 0; i < 10; i++){
  if(i % 2 == 0){
    str += i
  }
}

console.log(str);
```


4. for문을 사용하여 0부터 10미만의 정수 중에서 홀수만을 큰수부터 출력하시오.


output


```
9
7
5
3
1
```


Answer


```javascript

for(i = 10; i > 0; i--){
  if(i % 2 !== 0) 
    console.log(i);
}
```


5. while문을 사용하여 0 부터 10 미만의 정수 중에서 짝수만을 작은 수부터 출력하시오.


Output


```
0
2
4
6
8
```


Answer


```javascript
let i = 0;
while(i < 10){
  if(i % 2 == 0) console.log(i);
  i++;
}
```


6. while문을 사용하여 0 부터 10 미만의 정수 중에서 홀수만을 큰수부터 출력하시오.
   

Output


```
9
7
5
3
1
```

Answer


```javascript
let i = 9;
while(i > 0){
  if(i % 2 !== 0) console.log(i);
  i--;
}
```


7. for 문을 사용하여 0부터 10미만의 정수의 합을 출력하시오.


Output


```
45
```


Answer


```javascript
sum = 0;
for(let i = 0; i < 10 ; i++){
  sum += i;
}
console.log(sum)
```


8. 1부터 20 미만의 정수 중에서 2 또는 3의 배수가 아닌 수의 총합을 구하시오.


Output


```
73
```


Answer


```javascript
sum = 0;
for(let i = 1; i < 20; i++){
  if(!(i % 2 == 0) && !(i % 3 == 0)){
    sum += i;
  }
}
console.log(sum)
```


9. 1부터 20 미만의 정수 중에서 2 또는 3의 배수인 수의 총합을 구하시오.
    

Output


```
117
```


Answer


```javascript
sum = 0;
for(let i = 1; i < 20; i++){
  if(i % 2 == 0 || i % 3 == 0){
    sum += i;
  }
}
console.log(sum)
```


10. 두 개의 주사위를 던졌을 때, 눈의 합이 6이 되는 모든 경우의 수를 출력하시오.


Ouput


```
[ 1, 5 ]
[ 2, 4 ]
[ 3, 3 ]
[ 4, 2 ]
[ 5, 1 ]
```


Answer


```javascript
for(let i = 6; i > 0; i--){
  for(let n = 1; n < 6; n++){
    if(i + n == 6){
      console.log([i, n]);
    }
  }
}
```