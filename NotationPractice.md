1. O(n)
2. O(n)
3. O(1)
4. O(n^2) O(n^3)
5. O(n)
6. O(n^2) O(n)
7. O(n^2) O(n log n)
8. O(2^n)
9. O(1)
10. O(n^2)

Step Two:
```js
function logUpTo(n) {
  for (let i = 1; i <= n; i++) {
    console.log(i);
  }
}
```

Time Complexity: O(n)

```js
function logAtLeast10(n) {
  for (let i = 1; i <= Math.max(n, 10); i++) {
    console.log(i);
  }
}
```
Time Complexity: O(n)

```js
function logAtMost10(n) {
  for (let i = 1; i <= Math.min(n, 10); i++) {
    console.log(i);
  }
}
```

Time Complexity: O(1)

```js
function onlyElementsAtEvenIndex(array) {
  let newArray = [];
  for (let i = 0; i < array.length; i++) {
    if (i % 2 === 0) {
      newArray.push(array[i]);
    }
  }
  return newArray;
}
```

Time Complexity: O(n)

```js
function subtotals(array) {
  let subtotalArray = [];
  for (let i = 0; i < array.length; i++) {
    let subtotal = 0;
    for (let j = 0; j <= i; j++) {
      subtotal += array[j];
    }
    subtotalArray.push(subtotal);
  }
  return subtotalArray;
}
```
Time Complexity: O(n^2)
```js
function vowelCount(str) {
  let vowelCount = {};
  const vowels = "aeiouAEIOU";

  for (let char of str) {
    if(vowels.includes(char)) {
      if(char in vowelCount) {
        vowelCount[char] += 1;
      } else {
        vowelCount[char] = 1;
      }
    }
  }

  return vowelCount;
}
```
Time Complexity: O(n)

Part Three:

True or false: n^2 + n is O(n^2). True 
True or false: n^2 * n is O(n^3). False. (True) 
True or false: n^2 + n is O(n). False.
What’s the time complexity of the .indexOf array method? O(n)
What’s the time complexity of the .includes array method? O(n)
What’s the time complexity of the .forEach array method? O(n)
What’s the time complexity of the .sort array method? O(n log n)
What’s the time complexity of the .unshift array method? O(n log n) O(n)
What’s the time complexity of the .push array method? O(n) O(1)
What’s the time complexity of the .splice array method? O(n)
What’s the time complexity of the .pop array method? O(n) O(1)
What’s the time complexity of the Object.keys() function? O(n)
BONUS

What’s the space complexity of the Object.keys() function? O(n^2)??