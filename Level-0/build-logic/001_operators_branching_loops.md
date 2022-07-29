# Operators, Branching, Loops

## Easy

1. Write a program to add 5 numbers. The value of numbers are num1=5, num2=13, num3=7, num4=21 and num5=48.
```javascript
    const sumOfFive = (num1, num2, num3, num4, num5) => {
        return num1 + num2 + num3 + num4 + num5;
    };
    console.log(sumOfFive(5, 13, 21, 47, 48));
```

2. Write a program to take a number input from user and determine whether the number is odd or even.
```javascript
    const checkNumType = (inputNum) => {
     return inputNum % 2 === 0 ? "even" : "Odd";
    };
    console.log(checkNumType(8));
```
3. Write a program to find the maximum and minimum out of two given numbers. The numbers are num1=129 and num2=251.
```javascript
    const checkMaxAndMin = (num1, num2) => {
        const Maximum = Math.max(num1, num2);
        const Minimum = Math.min(num1, num2);
    console.log(`Maximum is : ${Maximum}, and minimum is : ${Minimum}`);
    };
checkMaxAndMin(129, 251);
```
- Find Minimum value from an Array
```javascript
 const arr = [10, 12, 14, 16, 18, 2];
 const minArray = Math.min(...arr);
 console.log(`Min. value from "array" is : ${minArray}`);
```
4. Write a program to find the maximum out of three given numbers. The numbers are num1=8, num2=23 and num3=17.
```jsx
const maxOfThree = (num1, num2, num3) => {
  const largestNum = Math.max(num1, num2, num3);
  console.log(`largest Number among 3 - using Math.max() is : ${largestNum}`);
};
maxOfThree(8, 23, 17);
```
5. Write a program to find the minimum out of three given numbers. The numbers are num1=35, num2=29 and num3=46.
```jsx
const minOfThree = (num1, num2, num3) => {
  // here added check for same inputs if given.
  if (num1 !== num2 || num2 !== num3 || num1 !== num3) {
    if (num1 <= num2 && num1 <= num3) {
      console.log(`${num1} is lowest among all 3`);
    } else if (num2 <= num3 && num2 <= num1) {
      console.log(`${num2} is lowest num among all 3`);
    } else {
      console.log(`${num3} is lowest number among all 3`);
    }
  } else {
    console.log("enter different numbers");
  }
};
minOfThree(35, 39, 46);
```
6. Write program to take a month as an input from the user and find out whether the month has 31 days or not. [repl solution](https://replit.com/@Vaibhav18Matere/get-days-in-month#index.js)

## Intermediate

1. Fizzbuzz - Write a program to return an array from 1 to 100. But for every multiple of 3, replace the number with "Fizz", for every multiple of 5, replace the number with "Buzz" and for every multiples of 3 & 5, replace with "FizzBuzz".

    Your output should look something like this `1, 2, Fizz, 4, Buzz, Fizz, 7, 8, Fizz, Buzz, 11, Fizz, 13, 14, FizzBuzz, 16, 17 ..... `

1. Print the following star pattern :-

    \* \
    \* \* \
    \* \* \* \
    \* \* \* \* \
    \* \* \* \* \*

1. Write a program to take a number input from user and print multiplication table 12 times for that number.

1. Write a program to return a Fibonacci series : 0,1,1,2,3,5,8,13,21.... [solution](https://replit.com/@Vaibhav18Matere/Neoggreater-fibonachi-series#script.js)

1. Write a program to take an input from a user and find its Factorial.
   `Example: Factorial of 5 is 120`
1. Write a Program to take a number input from user and find if the number is Prime or not.

1. Write a program to take a day as an input and determine whether it is a weekday or weekend.
   `Example: Tuesday is weekday.`
