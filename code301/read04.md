# Readings: React and Forms

![reactandform](https://res.cloudinary.com/practicaldev/image/fetch/s--KpQnReJ9--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://i1.wp.com/blogreact.com/wp-content/uploads/2020/03/forms.jpg%3Ffit%3D750%252C393%26ssl%3D1)

## React and Forms 

### 1. What Is A Controlled Component? 
A controlled component is essentially an input element that is fully controlled by React. 

### 2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why. ### 
I feel that it is better to have a controlled component and for the form to update the state with user responses as they type so that you can provide instant validation and and create custom instant formate. I feel that it is as though you have more control over React this way, instead of an uncontrolled way - where you might have to read the value before you can use it. It is more effiecient to have a an updating state as the user interacts. 

### 3.How do we target what the user is entering if we have an event handler on an input field? ### 

To target a users interaction with an input field you can use attributes to target the specific element, then you can use the event handler to handle that target event. 

By using value attributes that have a value in the state, then saving the targeted ``value`` in the state ``{value: event.target.value}``



## The Conditional (Ternary) Operator Explained

### 1.Why would we use a ternary operator? 
In a simiplied explanation, we would want to use a ternary operation if there are 3 opperands being used. A ternary is ultimately returns a boolean value and so if a condition is true then it will return an expression that is attached else the other expression. 