# 80s High School RPG

## By Andrew Philpott, Steven Fleming, Jose Amesquita and Jiwon Han Last updated April 15, 2020.

[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
![LastCommit](https://img.shields.io/github/last-commit/Andrew-Philpott/80s-rpg-game)
![Languages](https://img.shields.io/github/languages/top/Andrew-Philpott/80s-rpg-game)
[![MIT license](https://img.shields.io/badge/License-MIT-orange.svg)](https://lbesson.mit-license.org/)

#### 4/15/20 Work at Home Summary

- Design characters in game and test specifications

## Description

A RPG game.

## Specifications

## SPECS

| spec behavior                                                                | input                            | output                          |
| :--------------------------------------------------------------------------- | :------------------------------- | :------------------------------ |
| this                                                                         | that                             | the other                       |
| compare atheleticism between two Characters and return winner                | Nerd v Jock                      | Jock wins                       |
| compare cool between two Characters and return winner                        | Nerd v Jock                      | Jock wins                       |
| compare knowledge between two Characters and return winner                   | Nerd v Jock                      | Nerd wins                       |
| compare knowledge between two Characters of the same level and return winner | Nerd v Nerd                      | Nerds tie                       |
| winning Characters increase their level 2                                    | Vitality: 10 => W                | Vitality: 12                    |
| losing Characters decrease their level                                       | Vitality: 10 => L                | Vitality: 9                     |
| If they tie, they both lose a level                                          | Vitality P1: 10, Vitality P2: 10 | Vitality P1: 11, Vitality P2:11 |

## Setup/Installation Requirements

- Clone this [repository](https://github.com/Andrew-Philpott/80s-rpg-game.git)

## Known Bugs

No known bugs at this time.

## Support and contact details

Email or jiwon1.han@gmail.com with any questions, feedbacks, or concerns.

## Technologies Used

- Webpack
- Node.js

### License

This console application is licensed under the MIT license.

Copyright (c) 2020 **Andrew Philpott, Steven Fleming, Jose Amesquita and Jiwon Han**

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below 1000.

Create an array based off the value of the given number
if the number is divisible by 3 push to array, same for 5
sum the array

let arr = [];
let sum = 0;

for(let i = 0; i <= 1000; i++){
if(i % 3 === 0 || i % 5 === 0 ) {
sum += i
}
}
return sum;

function returnSum() {
let sum = 0;
for(let i = 0; i < 1000; i++){
if(i % 3 == 0 || i % 5 == 0 ) {
sum += i;
}
}
return sum;
}

//

Each new term in the Fibonacci sequence is generated by adding the previous two terms. By starting with 1 and 2, the first 10 terms will be:

0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...

By considering the terms in the Fibonacci sequence whose values do not exceed four million, find the sum of the even-valued terms.

for (i = 0; i <= param; i++){
}

//param is 400000000
returnEvenNumberFibonacciSum(param) {
let sum = 2;
//add
let fibonacciSequence = [0,1,2];

for (i = 2; i <= param; i++){
let NextNum = (fibonacciSequence[i-1]) + fibonacciSequence[i];
fibonacciSequence.push(NextNum);

    if((fibonacciSequence[i+1] != null) && (fibonacciSequence[i+1] % 2 === 0)) {
      sum += fibonacciSequence[i+1];
    }

}
return sum;
}

    // for (j= 0; j <= fibonacciSequence.length; j++)
      if(fibonacciSequence[j] % 2 === 0)
        sum += fibonacciSequence[j];



function returnEvenNumberFibonacciSum(param) {
let sum = 2;
let fibonacciSequence = [0,1,2];

for (let i = 2; i <= param; i++){
let NextNum = (fibonacciSequence[i-1] + fibonacciSequence[i]);
fibonacciSequence.push(NextNum);
console.log("next num" + NextNum);
if((fibonacciSequence[i+1] !== null) && (fibonacciSequence[i+1] % 2 == 0)) {
sum += fibonacciSequence[i+1];
console.log("sum" + sum);
}
}
return sum;
}

let i = 2;
while (sum <= param){
let NextNum = (fibonacciSequence[i-1] + fibonacciSequence[i]);
fibonacciSequence.push(NextNum);
console.log("next num" + NextNum);
if((fibonacciSequence[i+1] !== null) && (fibonacciSequence[i+1] % 2 == 0)) {
sum += fibonacciSequence[i+1];
console.log("sum" + sum);
}
i++;
}
return sum;
}

alert(returnEvenNumberFibonacciSum(10));
