# Spread Operator ```...```

``(...)``

The spread operator is a useful and quick syntax for **adding** items to arrays, **combining** arrays or objects, and **spreading** an array out into a functionβs arguments.

```js
Math.max(1,3,5) // 5
Math.max([1,3,5]) // NaN
Math.max(...[1,3,5]) // 5 
//The spread syntax βspreadsβ the array into separate arguments.
```

* splitting a string into characters, and combining the properties of two JavaScript objects:

```js

[...["ππππ€ͺπ"]] // Array [ "ππππ€ͺπ" ]
[..."ππππππ₯°ππ€©!"] // Array(9) [ "π", "π", "π", "π", "π", "π₯°", "π", "π€©", "!" ]

const hello = {hello: "ππππ€ͺπ"}
const world = {world: "ππππππ₯°ππ€©!"}

const helloWorld = {...hello,...world}
console.log(helloWorld) // Object { hello: "ππππ€ͺπ", world: "ππππππ₯°ππ€©!" }
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