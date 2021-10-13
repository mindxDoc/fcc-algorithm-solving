# Find the Longest Word in a String

Return the length of the longest word in the provided sentence.

Your response should be a number.

### 1. Answers

```javascript
function findLongestWord(str) {

  var arr = str.split(' ');

  var max = 0;

  for (var i = 0; i < arr.length; i++) {
    var valStr = arr[i].length;

    if (valStr > max) {
      max = valStr;
    }
  }
  return max;
}

findLongestWord("The quick brown fox jumped over the lazy dog");
```

### 2. Explain

1. We create a arr with the str
2. Setup a var for tracked the length of the bigger
3. Loop inside the arr
4. Setup a var for shortcut the length
5. If the new one is bigger than the prev one make it the new bigger