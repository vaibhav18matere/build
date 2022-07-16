1. Given a and b, your function should return the value of a^b
2. Given an array, your function should return the length of the array.
3. Write a function that generates a secret code from a given string, by shifting characters of the alphabet by N places. Example:
- Input: encodeString("neogcamp", 2) ––> Output: pgqiecor
- Explanation: 2 represents shifting alphabets by 2 places. a –> c, b –> d, c –> e and so on.
4. Given length of a regular hexagon, your function should return area of the hexagon.
5. Given an array and an item, your function should return the index at which the item is present.
6. Given a sentence, return a sentence with first letter of all words as capital.
7. Given a sentence, your functions should return the number of words in the sentence.
8. Given an array and two numbers, your function should replace all entries of the first number in an array with the second number.
9. Given an array of numbers, your function should return an array in the ascending order.
- Input: sortArray([100,83,32,9,45,61]) ––> Output: [9,32,45,61,83,100]
10. Given n numbers, your function should return the minimum of them all. The number of parameters won't be accepted from user.
- Input: findMin(3,5) ––> Output: 3
- Input: findMin(3,5,9,1) ––> Output: 1
11. Given two arrays, your function should return single merged array.
- Input: mergeArray([1,3,5], [2,4,6]) ––> Output: [1,3,5,2,4,6]
12. Given a sentence, your function should reverse the order of characters in each word, keeping the same sequence of words.
- Input: reverseCharactersOfWord('we are neoGrammers') –––> Output: ew era sremmarGoen
13. Write a program that takes two strings and copies smaller strings into a bigger string.
14. Write a program that converts the string into uppercase.
15. Given an input string S and two characters c1 and c2, you need to replace every occurrence of character c1 with character c2 in the given string.
16. A program that reads a string and counts the number of characters present in the string.
17. Write a program that removes the time from the given date string "Wed April 15, 7 pm". It should return only the date without the time.
18. Given an input string S that contains multiple words, you need to remove all the spaces present in the input string. There can be multiple spaces present after any word.
19. Write a program that masks all but the last four characters of the string "5565534276455423" to '#'
20. Given a string, determine if it is a palindrome, considering only alphanumeric characters
21. Reverse the given string word wise. That is, the last word in a given string should come at 1st place, the last-second word at 2nd place and so on. Individual words should remain as it is. example: Input: Welcome to neoG Camp → Camp neoG to Welcome
22. Given n numbers, your function should return the maximum of them all. The number of parameters won't be accepted by the user. Example:Input: findMax(3,5) ––> Output: 5Input: findMax(3,5,9,1) ––> Output: 9
(Hint: Lookup rest parameters in JavaScript)
23. Given a string and an index, your function should return the character present at that index in the string.Example:Input: charAt("neoGcamp", 4) ––> Output: c
24. Write a program to take a day as input and determine whether it is a weekday or weekend. Example: Tuesday is weekday.
25. Given three angles of a triangle, your function should return if it is a scalene, isosceles, equilateral triangle or not a triangle at all. Example: Input: typeOfTriangle(30, 60, 90) ––> Output: Scalene Triangle
26. Given two dates, your function should return which one comes before the other. 
- Input: minDate('02/05/2021', '24/01/2021') ––> Output: 24/01/2021
27. A program that counts the value of each character and prints the most repeated character?
28. Given the Cost Price(CP) and Selling Price(SP) of a product. Write a Program to Calculate the Profit or Loss.
- Input: CP = 1500, SP = 2000
- Output: 500 Profit
- Input: CP = 3125, SP = 1125
- Output: 2000 Loss`
29. Write a JavaScript program to compute the sum of all digits that occur in a given string.
30. Write a Program to convert Decimal to Binary.
31. Calculate the area and perimeter of a square of side 'a'. Also, calculate the surface area and the volume of a cube of side 'a'
32. Write a Program to Print N Odd Number in Descending Order.
33. Write a Program to cyclically Rotate a Number by X positions in the left direction, as provided by the user.
- Enter a Number: 1234
- Enter the Number of Rotations: 2
- Output: 3412`
34. Write a program to convert Fahrenheit to Celsius. For Fahrenheit to Celsius conversion use: `C = (F - 32) * 5/9` 'F' and 'C' are the temperatures on the Fahrenheit scale and Celsius scale respectively.
- Input: 56
- Output: 13.33333`
35. Write a program to calculate the sum of N natural digits, as input by the users?
36. Write a JavaScript program that reverses a number.
37. Write a program to calculate the kinetic energy of a body with mass 'm' and volume 'v'.
- Formula : `0.5 * m * v * v`
38. Write a JavaScript program to calculate the simple interest given P,R,T with the given formula. 
- Formula: `SI = (P * T * R) / 100` Where: P = principal amount T = time R = rate SI = simple interest 
- Input: P=100, R=6%, T=2
- Output: 12`
39. Write a Program to Convert Octal to Decimal.
- Enter an octal number: 116
- Octal of Given Number = 78 in decimal`
40. Display the transpose of a matrix.
41. Given an object obj, we have to invert its key and value for each entry. Inversion will result in value being used as key and key as value.
- Note:- There will be no repeated values to maintain the uniqueness.
// Input:
obj = {
  "name" : "Doraemon",
	"age" : 5,
	"hairColor" : "none",
	"eyes" : "oval"
}

// Output:
obj = {
   "Doraemon" : "name",
		"5" : "age",
		"none" : "hairColor",
		"oval" : "eyes"
}
42. Given an array of numbers, pick any two numbers a  and b, we could get the difference by Math.abs(a - b) 
- Write a function to get the largest difference.
43. Given an array arr with different counts of numbers, we have to find the number with the most frequency and return it. 
If there are two or more numbers with the same most frequency they return the biggest number.
44. 1. Given an array of integer `nums` and an integer `target`, check if there are two numbers in the array such that they add up to `target`. Return any one pair that add up to the target
    
    ```jsx
    Input: nums = [3,7,11,15], target = 18
    Output: [3,15]
    Explanation : nus[0] + nums[3] = 18
    ```
45. 1. Given an array and size k, break the array into chunks of k-length and return them as an array.
    
    ```jsx
    Input: arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], k = 3
    Output: [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]
    ```
46. Given an array `arr` with different counts of numbers, we have to find the number with the least frequency and return it.
If there are two or more numbers with the same least frequency they return the biggest number.
- Input: arr = [2, 2, 2, 3, 3, 3, 4, 4, 4, 2, 5, 5, 5, 6, 6,8,8]
- Output: 8
47. Given an integer array nums, move all 0's to the end of it while maintaining the relative order of the non-zero elements.
- Input: nums = [0,2,0,3,12,0]
- Output: [2,3,12,0,0,0]
48. Given an array nums with length n, return the element which occurred at least n/2 times in the array.
- Input: nums = [2,2,1,1,1,2,2]
- Output: 2
49. Given a string s, find the first non-repeating character in it and return its index If it does not exist, return -1 
- Input: s = "neogcamp"
- Output: "n"
- Input: s = "nneeooggccaammpp"
- Output: -1
50. Given a valid (IPv4) IP `address`, return a defanged version of that IP address.
- A *defanged IP address* replaces every period `"."` with `"[.]"`.
- Input: address = "255.100.50.0"
- Output: "255[.]100[.]50[.]0"
51. Given a string `s`, reverse only all the vowels in the string and return it.
- The vowels are `'a'`, `'e'`, `'i'`, `'o'`, and `'u'`, and they can appear in both cases. 
- Input: s = "neoGCamp"
- Output: "naoGCemp"
52. You have been given a string `summerFruits` that are available in summer, and `fruits`
 representing the fruits you have. Find the summer fruits in the fruits. 
- `summerFruits` is case-sensitive. `(a is not equal to A)`. 
- Each character represents a type of fruit and the fruits present in the summer fruits are unique.
- `Input:` `summerFruits = "aA", fruits = "aaAAbbbb"
- Output: 4`
53. Given a string, str, return the length of the last word.
     - ex: "hello neoGrammers" -> 11,
     - ex: "hello neoGrammers you guys rock" -> 4
54. Given two strings check if the second string is an anagram of first.
- ex: s1="below" s2= "elbow" -> true,
- ex: s1="gain" s2="pain" -> false
55. Given two strings check if the first string can match the second string after some number of shifts.
- ex: s1 = "xyza", s2= "zaxy" -> true
- s1 = "xyza", s2= "yzxa" -> false
56. Write a program to take a month as input from the user and find out whether the month has 31 days or not.
57. Find the number of consonants and vowels in a string.
58. Fizzbuzz - Write a program to return an array from 1 to 100. But for every multiple of 3, replace the number with "Fizz", for every multiple of 5, replace the number with "Buzz" and for every multiple of 3 & 5, replace it with "FizzBuzz".
- Your output should look something like this
- `1, 2, Fizz, 4, Buzz, Fizz, 7, 8, Fizz, Buzz, 11, Fizz, 13, 14, FizzBuzz, 16, 17 .....`
59. You are given an `n x n` 2D `matrix` representing an image, rotate the image by **90** degrees (clockwise).
- Input: matrix = [[1,2,3],[4,5,6],[7,8,9]]
- Output: [[7,4,1],[8,5,2],[9,6,3]]
60. Given a 2D integer array matrix, return the transpose of matrix. The transpose of a matrix is the matrix flipped over its main diagonal, switching the matrix's row and column indices
- Input: matrix = [[1,2,3],[4,5,6],[7,8,9]]
- Output: [[1,4,7],[2,5,8],[3,6,9]]
61. You are given an m x n   integer grid accounts where accounts[i][j] is the amount of money the ith customer has in the jth  bank. Return the wealth that the richest customer has.  A customer's wealth is the amount of money they have in all their bank accounts. The richest customer is the customer that has the maximum wealth.
- Input: accounts = [[1,2,3],[3,2,1]]
- Output: 6
62. Given an `n x n` binary matrix `image`, flip the image **horizontally**, then invert it, and return *the resulting image*.
- To flip an image horizontally means that each row of the image is reversed.
- For example, flipping `[1,1,0]` horizontally results in `[0,1,1]`.
- To invert an image means that each `0` is replaced by `1`, and each `1` is replaced by `0`.
- For example, inverting `[0,1,1]` results in `[1,0,0]`.
- Input: image = [[1,1,0],[1,0,1],[0,0,0]]
- Output: [[1,0,0],[0,1,0],[1,1,1]]
- Explanation: First reverse each row: [[0,1,1],[1,0,1],[0,0,0]].
- Then, invert the image: [[1,0,0],[0,1,0],[1,1,1]]
63. Given the array `prices` where `prices[i]` is the price of the `ith` item in a shop. 
- There is a special discount for items in the shop, 
- if you buy the `ith` item, then you will receive a discount equivalent to `prices[j]` where `j` is the **minimum** index such that `j > i` and `prices[j] <= prices[i]`, 
- otherwise, you will not receive any discount at all.
- *Return an array where the `ith` element is the final price you will pay for the `ith` item of the shop considering the special discount.*
- Input: prices = [8,4,6,2,3] {`Mango`: 8, `Cherry`: 14, `Banana`: 6, `Chickoo`: 2, `Apple`: 3}}
- Output: [4,2,4,2,3]
- Explanation: 
     - For item 0 with price[0]=8 you will receive a discount equivalent to prices[1]=4, therefore, the final price you will pay is 8 - 4 = 4. 
     - For item 1 with price[1]=4 you will receive a discount equivalent to prices[3]=2, therefore, the final price you will pay is 4 - 2 = 2. 
     - For item 2 with price[2]=6 you will receive a discount equivalent to prices[3]=2, therefore, the final price you will pay is 6 - 2 = 4. 
     - For items 3 and 4 you will not receive any discount at all.
- Input: prices = [1,2,3,4,5]
- Output: [1,2,3,4,5]
- Explanation: In this case, for all items, you will not receive any discount at all.
- Input: prices = [10,1,1,6]
- Output: [9,0,1,6]
64. You are keeping score for a baseball game with strange rules. The game consists of several rounds, where the scores of past rounds may affect future rounds' scores.
- At the beginning of the game, you start with an empty record. You are given a list of strings ops, where ops[i] is the ith operation you must apply to the record and is one of the following:
- An integer x - Record a new score of x.
- "+" - Record a new score that is the sum of the previous two scores. It is guaranteed there will always be two previous scores.
- "D" - Record a new score that is double the previous score. It is guaranteed there will always be a previous score.
- "C" - Invalidate the previous score, removing it from the record. It is guaranteed there will always be a previous score.
- Return the sum of all the scores on the record.
- Input: ops = ["5","2","C","D","+"]
- Output: 30
- Explanation:
     - "5" - Add 5 to the record, record is now [5].
     - "2" - Add 2 to the record, record is now [5, 2].
     - "C" - Invalidate and remove the previous score, record is now [5].
     - "D" - Add 2 * 5 = 10 to the record, record is now [5, 10].
     - "+" - Add 5 + 10 = 15 to the record, record is now [5, 10, 15].
     - The total sum is 5 + 10 + 15 = 30.