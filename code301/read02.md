# Readings: State and Props

![react](https://res.cloudinary.com/practicaldev/image/fetch/s--xKWyj8SG--/c_imagga_scale,f_auto,fl_progressive,h_500,q_auto,w_1000/http://live-linguine-code.pantheonsite.io/wp-content/uploads/2019/03/react-state-vs-props.jpg)

```js
class FishTableRow extends React.Component {
constructor() {
super(props); //gives us access to props
//Don’t call this.setState() here
this.state = { //intitialize local state
showDescription: false
} 
}
```

**Avoid using this.setState() in the constructor because it can lead to side effects, and it is unnecessary. Doing this will ignore all updates to props, so it shouldn’t be done unless it is intentional.**

## React lifecycle

* Lifecycles are the methods that you use on the classes and functions in react.

1. In the diagram the render happened before the componentDidMount.

2. The first thing that happens in the lifecycle of react is Mounting. Mounting is when an instance of a compoenent is made and put into the DOM.

3. **The order is Constructor>render>React updates >componentDidMount>componentWillUnmount**

4. If you need to load anything using a network request or initialize the DOM, it should go here.

----------


* What types of things can you pass in the props?

Numbers, strings, functions

* What's the big difference between props and state?

Props passed into the component and handled outside the component, but states handled inside the component.


* When do we re-render our application?

When the state is changed inside the application it will re-render the application.

* What are some examples of things that we could store in state?

A counter count can be stored in state, inside a form where things are updated by a user. (counter and form inputs)


## Things I want to know more about