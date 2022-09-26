# core-code-upskilling-readme
## Week challenges

### `Thursday 09/22/2022`
##### 1. React Santa Wish List  
```js
class WishlistForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = { name:'', wish:'', priority:1 }
    this.handleSubmit = this.handleSubmit.bind(this);
  }
  
  handleSubmit(e){
    e.preventDefault()
    this.props.send(this.state)
  }
  
  render() {
    return (
      <form onSubmit={this.handleSubmit}>
        <input id="name" onChange={(e)=>this.setState({name: e.target.value})}/>
        <textarea type="textarea" id="wish"  onChange={(e)=>this.setState({wish: e.target.value})}/>
        <select name="priority" id="priority" value={this.state.priority} onChange={(e)=>this.setState({priority: e.target.value})}>
          <option value="1">1</option>
          <option value="2">2</option>
          <option value="3">3</option>
          <option value="4">4</option>
          <option value="5">5</option>
        </select>
      </form>
    );
  }
};
```

### `Wednesday 09/21/2022`
##### 1. React Manage Events  
```js
export class Counter extends React.Component {
  constructor(props) {
    super()
    this.state = { counter: 0}
  }
  
  render() {
    return (
      <div>
        <h1 id="counter">{this.state.counter}</h1>
          <button id="decrement" type="button" onClick={()=>this.setState({ counter: this.state.counter -1})}>
            Decrement
          </button>
          <button id="increment" type="button" onClick={()=>this.setState({ counter: this.state.counter + 1})}>
            Increment
          </button>
      </div>
    )
  }
}
```

### `Tuesday 09/20/2022`
##### 1. Well Of Ideas  
```js
function well(x){
  const goodIdeas = x.filter( i => i==='good').length
  if(goodIdeas > 2){
    return 'I smell a series!'
  }else if( goodIdeas > 0){
    return 'Publish!'
  }else{
    return 'Fail!'
  }
}
```

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
