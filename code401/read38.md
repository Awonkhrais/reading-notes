## React Conditional rendering

Creating a component that encapsulates behavior you need, and only have them render depending on the state of the application

**Element Variables**

Element variables help conditionally render part of the component while the rest of the output remains the same


## List and Keys

**Basic List Component**

You will usually render lists inside components

* When you create a list using the map() function, you must assign them a key

- Keys help React identify changed,added and removed items. They also give each list item a valid identity
- Keys must be unique among siblings (do not have to be globally unique)

**Embedding map functions**

To embed a map function, you will use JSX syntax, using curly braces

## Forms

In React form elements naturally keep some internal state. Generally you will want to have a function that handles the submission of the form, and has access to the data that the user submitted

**Controlled Components**

In HTML, form elements (< input >, < textarea >, < select >, etc.) typically maintain their own state and update it based on user input

- In React mutable state will be kept in the state property of componenets and will be updated with setState()
- The React component renders a form, and also controls what happens in that form on subsequent user input. Forms that are controlled this way are "Controlled Components"


**Select tag**

In react, select is used for a dropdown list. Each < option > within the select tag is an option in the list


## Lifting state

When several components need to reflect the same changed data you will need to lift state

- In order to lift state up, you will remove "local state" from a component, and add it the common closest ancestor that it needs to share changes with
- Since the state will be coming from a parent, it will now be a prop
- Instead of calling setState(), you will call this.props.function(), which is provided by the parent component

## Composition vs Inheritance

React's composition model is recommended for reuse of code between components

- In order to let components know of child components ahead of time, you can use the "children" prop to pass children elements directly into their output

## Thinking in React

1. Start with a mock (JSON API and Mock from a designer)
2. Break the UI into a component hierarchy (draw boxes around every component, and subcomponent in the mock, and figure out which components appear within another component)
3. Build a static version
4. Identify MVP representation of UI State
5. Identify where state lives
6. Add inverse data flow