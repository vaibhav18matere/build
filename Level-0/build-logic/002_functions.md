# Functions

## Easy

1. Given a and b, your function should return the value of a<sup>b</sup>  
**Example:**  
**Input:** `power(2,3)` ––> **Output:** `8`
```jsx
const aPowerB = (a, b) => Math.pow(a, b);
console.log(aPowerB(2, 3));
```
- another approch
```jsx
const aRaisedToB = (a, b) => a ** b;
console.log(aRaisedToB(2, 4));
```
1. Given length of a regular hexagon, your function should return area of the hexagon.  
**Example:**  
**Input:** `areaOfHexagon(10)` ––> **Output:** `259.80`
```jsx
const hexagonConst = (3 * Math.sqrt(3)) / 2;

const areaOfHexagon = (side) => {
  const area = hexagonConst * Number(side ** 2);
  return area.toFixed(2);
};

console.log(areaOfHexagon(10));
```
1. Given a sentence, your functions should return the number of words in the sentence.  
**Example:**  
**Input:** `noOfWords(We are neoGrammers)` ––> **Output:** `3`
```jsx
const numberOfWords = (inputGiven) => {
  if (inputGiven == null || inputGiven.length === 0) {
    console.log(0);
  } else {
    const totalWords = inputGiven.split(" ").length;
    console.log(totalWords);
  }
};
numberOfWords("We are neoGrammers");
```
```jsx
function countWords(str) {
  // Check if the string is null or empty then return zero
  if (str == null || str.length === 0) return 0;

  let wordCount = 0;

  let isWord = false;
  let endOfLine = str.length - 1;

  // Converting the given string into a character array
  let ch = str.split("");

  for (let i = 0; i < ch.length; i++) {
    if (isLetter(ch[i]) && i !== endOfLine) isWord = true;
    // Check if the character is a letter
    // and index of character array doesn't equal to end of line
    // that means, it is a word and set isWord by true.
    else if (!isLetter(ch[i]) && isWord) {
      wordCount++;
      isWord = false;

      // Check if the character is not a letter
      // that means there is a space, then we
      // increment the wordCount by one and set
      // the isWord by false
    } else if (isLetter(ch[i]) && i === endOfLine) wordCount++;
    // Check for the last word of the sentence and
    // increment the wordCount by one
  }
  return wordCount;
}

function isLetter(c) {
  return c.toLowerCase() !== c.toUpperCase();
}

console.log(("No of words : " + countWords("Zero One two three four five")));
```
1. Given n numbers, your function should return the minimum of them all. The number of parameters won't be accepted from user.  
**Example:**  
**Input:** `findMin(3,5)` ––> **Output:** `3`  
**Input:** `findMin(3,5,9,1)` ––> **Output:** `1`  
*(Hint: Lookup rest parameters in JavaScript)*
1. Given n numbers, your function should return the maximum of them all. The number of parameters won't be accepted from user.  
**Example:**  
**Input:** `findMax(3,5)` ––> **Output:** `5`  
**Input:** `findMax(3,5,9,1)` ––> **Output:** `9`  
*(Hint: Lookup rest parameters in JavaScript)*
1. Given three angles of a triange, your function should return if it is a scalene, isosceles, equilateral triangle or not a triangle at all.
**Example:**  
**Input:** `typeOfTriangle(30, 60, 90)` ––> **Output:** `Scalene Triangle`

## Medium

1. Given an array, your function should return the length of the array.  
**Example:**  
**Input:** `arrayLength([1,5,3,7,8])` ––> **Output:** `5`
1. Given an array and an item, your function should return the index at which the item is present.  
**Example:**  
**Input:** `indexOf([1,6,3,5,8,9], 3)` ––> **Output:** `2`
1. Given an array and two numbers, your function should replace all entries of first number in an array with the second number.  
**Example:**  
**Input:** `replace([1,5,3,5,6,8], 5, 10)` ––> **Output:** `[1,10,3,10,6,8]`
1. Given two arrays, your function should return single merged array.  
**Example:**  
**Input:** `mergeArray([1,3,5], [2,4,6])` ––> **Output:** `[1,3,5,2,4,6]`
1. Given a string and an index, your function should return the character present at that index in the string.  
**Example:**  
**Input:** `charAt("neoGcamp", 4)` ––> **Output:** `c`
1. Given two dates, your function should return which one comes before the other.  
**Example:**  
**Input:** `minDate('02/05/2021', '24/01/2021')` ––> **Output:** `24/01/2021`

## Advanced

1. Write a function which generates a secret code from a given string, by shifting characters of alphabet by N places.
**Example:**  
**Input:** `encodeString("neogcamp", 2)` ––> **Output:** `pgqiecor`  
Explanation: 2 represents shifting alphabets by 2 places. a –> c, b –> d, c –> e and so on.
1. Given a sentence, return a sentence with first letter of all words as capital.  
**Example:**  
**Input:** `toSentenceCase('we are neoGrammers')` ––> **Output:** `We Are NeoGrammers`
1. Given an array of numbers, your function should return an array in the ascending order.  
**Example:**  
**Input:** `sortArray([100,83,32,9,45,61])` ––> **Output:** `[9,32,45,61,83,100]`
1. Given a sentence, your function should reverse the order of characters in each word, keeping same sequence of words.  
**Example:**  
**Input:** `reverseCharactersOfWord('we are neoGrammers')` –––> **Output:** `ew era sremmarGoen`
