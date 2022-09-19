# core-code-upskilling-readme
## Week challenges

### `Monday 09/19/2022`
##### 1. Is Palindrome? 
```js
function isPalindrome(line) {
  const word = line.toString();
  return word === word.split('').reverse().join('');
}
```

### `Thursday 09/15/2022`
##### 1. Odd Or Even
```js
function oddOrEven(array) {
  const sum = array.reduce( (a,b) => a+b, 0);
  return sum%2 === 0 ? "even" : "odd";
}
```

### `Wednesday 9/14/2022`
##### 1. Smallest Integer In Array 
```js
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return args.reduce((a,b)=>Math.min(a,b))
  }
}
```

### `Tuesday 9/13/2022`
##### 1. Ensure Question
```js
function ensureQuestion(s) {
  return s.endsWith('?') ? s : `${s}?`
}
```
##### 2. Reverse Sentence
```js
function reverseWords(str){
  return str.split(' ').reverse().join(" ")
}
```
