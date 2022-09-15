# core-code-upskilling-readme
## Week challenges

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
