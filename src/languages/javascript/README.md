# Fizzbuzz

## Description
Have the function `FizzBuzz(num)` take the `num` parameter being passed and return `all the numbers from 1 to num separated by spaces`, but replace every number that is divisible by 3 with the word "Fizz", replace every number that is divisible by 5 with the word "Buzz", and every number that is divisible by both 3 and 5 with the word "FizzBuzz".

**So for example:**
```
if num is 16
Your program should return the string "1 2 Fizz 4 Buzz Fizz 7 8 Fizz Buzz 11 Fizz 13 14 FizzBuzz 16". 
```
The input will be within the range 1 - 50.

## Examples
```
    Input: 3
    Output: 1 2 Fizz
    
    Input: 8
    Output: 1 2 Fizz 4 Buzz Fizz 7 8
```

## Solution
```javascript
function FizzBuzz(num) {
    let result = '';
    for(let i=1; i<=num; i++) {
        if(i%3 === 0 && i%5 === 0) result += ' FizzBuzz'
        else if(i%3 === 0) result += ' Fizz';
        else if(i%5 === 0) result += ' Buzz';
        else result += ` ${i}`;
    }
    return result.trim(); 
}
```

## Breaking down the solution
The code is clean, simple `for` statement to make **iterative** algorithm operation, the variable name `result` is used for the function result, and just for that.
In code knowledge, using `let` in JavaScript is a good practice, and also this solution shows a `ES6` (The current JavaScript standard) operation which is call [Template literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals) and you can see it on the statement: `else result += ` ${i}`;`

## Try it!
Click [here](https://jsbin.com/?js,console) to copy paste the code in a JavaScript environment, just copy the code and make the call with the number you want, in this example `8`, to run the code just hit the **Run** button on the right. 

```javascript

function FizzBuzz(num) {
    let result = '';
    for(let i=1; i<=num; i++) {
        if(i%3 === 0 && i%5 === 0) result += ' FizzBuzz'
        else if(i%3 === 0) result += ' Fizz';
        else if(i%5 === 0) result += ' Buzz';
        else result += ` ${i}`;
    }
    return result.trim(); 
}

// we are making the call and printing the result
console.log(FizzBuzz(8));

```