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

2. Given length of a regular hexagon, your function should return area of the hexagon.  
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

3. Given a sentence, your functions should return the number of words in the sentence.  
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
      // increment the wordCount by one
      // and set the isWord by false
    } else if (isLetter(ch[i]) && i === endOfLine) wordCount++;
    // Check for the last word of the sentence and
    // increment the wordCount by one
  }
  return wordCount;
}

function isLetter(c) {
  return c.toLowerCase() !== c.toUpperCase();
}

console.log("No of words : " + countWords("Zero One two three four five"));
```

4. Given n numbers, your function should return the minimum of them all. The number of parameters won't be accepted from user.  
    **Example:**  
    **Input:** `findMin(3,5)` ––> **Output:** `3`  
    **Input:** `findMin(3,5,9,1)` ––> **Output:** `1`  
   _(Hint: Lookup rest parameters in JavaScript)_

- Using defined method

```jsx
const findMin = (...args) => {
  console.log(Math.min(...args));
};
findMin(3, 5, 9, 1, 0, -8);
```

- Using for loop

```jsx
function findMin(...array) {
  var i = 0;
  var min = array[0];
  for (i = 1; i < array.length; i++) {
    if (array[i] < min) {
      min = array[i];
    }
  }
  return min;
}
console.log(findMin(3, 5, 9, 1));
```

- using Reducer

```jsx
const findMin = (...numbers) => {
  const min = numbers.reduce((previous, current) =>
    previous < current ? previous : current
  );
  return min;
};
console.log("Minimum out of all numbers: ", findMin(11, 5, 9, 1));
```

5. Given three angles of a triange, your function should return if it is a scalene, isosceles, equilateral triangle or not a triangle at all.
   **Example:**  
   **Input:** `typeOfTriangle(30, 60, 90)` ––> **Output:** `Scalene Triangle`

```jsx
const typeOfTriangle = (angle1, angle2, angle3) => {
  if (angle1 + angle2 + angle3 === 180) {
    if (angle1 === angle2 && angle2 === angle3) {
      console.log("Equilateral Triangle");
    } else if (angle1 === angle2 || angle2 === angle3 || angle1 === angle3) {
      console.log("Isoscale triangle");
    } else {
      console.log("Scalene Triangle");
    }
  } else {
    console.log("It's not a triangle");
  }
};

typeOfTriangle(90, 50, 40);
```

## Medium

1. Given an array, your function should return the length of the array.  
   **Example:**  
   **Input:** `arrayLength([1,5,3,7,8])` ––> **Output:** `5`

```jsx
const arrayLength = (arr) => {
  console.log(arr.length);
};
console.log(arrayLength([1, 5, 3, 7, 8]));
```

2. Given an array and an item, your function should return the index at which the item is present.
   **Example:**
   **Input:** `indexOf([1,6,3,5,8,9], 3)` ––> **Output:** `2`

```jsx
const indexOfNum = (arr, value) => {
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] === value) return i;
  }
};
console.log(indexOfNum([1, 6, 3, 5, 8, 9], 3));
```

3. Given an array and two numbers, your function should replace all entries of first number in an array with the second number.
   **Example:**
   **Input:** `replace([1,5,3,5,6,8], 5, 10)` ––> **Output:** `[1,10,3,10,6,8]`

```jsx
const replaceNumWith = (arr, num1, num2) => {
  for (let i = 0; i < arr.length; i++) {
    if (arr[i] == num1) {
      arr[i] = num2;
    }
  }
  return arr;
};

console.log(replaceNumWith([1, 5, 3, 5, 6, 8], 5, 10));
```

- Other approach

```jsx
const items = [1, 5, 3, 5, 6, 8];

const newItems = items.map((item) => (item === 5 ? 100 : item));

console.log(newItems);
```

4. Given two arrays, your function should return single merged array.
   **Example:**
   **Input:** `mergeArray([1,3,5], [2,4,6])` ––> **Output:** `[1,3,5,2,4,6]`

```jsx
const mergeArray = (arr1, arr2) => {
  return arr1.concat(arr2);
};

console.log(mergeArray([1, 3, 5], [2, 4, 6]));
```

```jsx
const mergedArray2 = (arr1, arr2) => {
  let NewmergedArray2 = [...arr1, ...arr2];
  console.log(NewmergedArray2);
};

mergedArray2([1, 2, 3], [4, 5, 6]);
```

5. Given a string and an index, your function should return the character present at that index in the string.
   **Example:**
   **Input:** `charAt("neoGcamp", 4)` ––> **Output:** `c`

```jsx
const findChatAtIndex = (strInput, IndexReq) => {
  const newArr = strInput.split(" ").join();
  //console.log(newArr);
  for (let i = 0; i < newArr.length; i++) {
    const result = newArr[IndexReq];
    console.log(result);
  }
};

findChatAtIndex("VaibhavMatere", 3);
```

6. Given two dates, your function should return which one comes before the other.
   **Example:**
   **Input:** `minDate('02/05/2021', '24/01/2021')` ––> **Output:** `24/01/2021`

```jsx
const minDate = (date1, date2) => {
  if (date1 > date2) {
    return date1;
  } else if (date1 < date2) {
    return date2;
  } else {
    return "both dates are same";
  }
};
console.log(minDate("02/05/2021", "24/01/2021"));
```

- using ternary operator

```jsx
const findMinDate = (date1, date2) => {
  return date1 > date2 ? date1 : date2 > date1 ? date2 : "both dates are same";
};
console.log(findMinDate("02/05/2021", "24/01/2021"));
```

## Advanced

1. Write a function which generates a secret code from a given string, by shifting characters of alphabet by N places.
   **Example:**
   **Input:** `encodeString("neogcamp", 2)` ––> **Output:** `pgqiecor`
   Explanation: 2 represents shifting alphabets by 2 places. a –> c, b –> d, c –> e and so on.

```jsx
console.log("function problem");
```

2. Given a sentence, return a sentence with first letter of all words as capital.
   **Example:**
   **Input:** `toSentenceCase('we are neoGrammers')` ––> **Output:** `We Are NeoGrammers`

```jsx
console.log("function problem");
```

3. Given an array of numbers, your function should return an array in the ascending order.
   **Example:**
   **Input:** `sortArray([100,83,32,9,45,61])` ––> **Output:** `[9,32,45,61,83,100]`

```jsx
console.log("function problem");
```

4. Given a sentence, your function should reverse the order of characters in each word, keeping same sequence of words.
   **Example:**
   **Input:** `reverseCharactersOfWord('we are neoGrammers')` –––> **Output:** `ew era sremmarGoen`

```jsx
console.log("function problem");
```
