# React Dos - Thinking in React

- How would you break a mock into a component heirarchy? **Firstly you would draw boxes around each componenet. Then you use the `single responisibilty principle` in which you decide that components should only do one thing.  If the component ends up doing more than one thing then you have to break it down even further into sub-components**
- What is the single responsibility principle and how does it apply to components? **It is a break down of the componenets into subcomponents if those components do more than one function or have more than one object.**
- What does it mean to build a ‘static’ version of your application?
**Building a static version of an app means that it has in interactivity so renders the data model. You do not use `state` because `state` is only for interactivity.**
- Once you have a static application, what do you need to add?
**You want to add props so that you can pass data from parent to child**
- What are the three questions you can ask to determine if something is state? 
**Is it passed in from a parent via props?Does it remain unchanged over time?Can you compute it based on any other state or props in your component?**

- How can you identify where state needs to live?
**dentify every component that renders something based on that state.Find a common owner component (a single component above all the components that need the state in the hierarchy).Either the common owner or another component higher up in the hierarchy should own the state.If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.**