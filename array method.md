# Spread Operator ```...```

``(...)``

The spread operator is a useful and quick syntax for **adding** items to arrays, **combining** arrays or objects, and **spreading** an array out into a function’s arguments.

```js
Math.max(1,3,5) // 5
Math.max([1,3,5]) // NaN
Math.max(...[1,3,5]) // 5 
//The spread syntax “spreads” the array into separate arguments.
```

* splitting a string into characters, and combining the properties of two JavaScript objects:

```js

[...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
[..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }
```

# The Conditional (Ternary) / if ternary

```js
let person = {
  name: 'tony',
  age: 20,
  driver: null
};
```

if :

```js
if (person.age >= 16) {
  person.driver = 'Yes';
} else {
  person.driver = 'No';
}
```

if ternary :


```js
person.driver = person.age >=16 ? 'Yes' : 'No' ;

```