# Classes and Objects

* Objects are an encapsulation of variables and functions into a single entity. Objects get their varaibles and functions from classes.
* A very basic class would look something like this: class MyClass:

 ```
 variable = "blah" 
 def function(self) 
    print("message")
 ```

* How to assign a class to an object: myobjectx = MyClass()

* You can use dot notation to accesst the variable inside the class. print(myobjectx.variable) would display "blah"

* You can create multiple different objects that are of the same class with the same variables and functions defined. However, each object contains independent copies of the variables defined in the class.

* myobjectx = MyClass(), myobjecty = MyClass(), myobjecty.variable = "yackity"

* To access a funciton inside of an object you use dot notation. myobjectx.function().

--------------------------------------------------

# Thinking recursively

A recursive function is a function defined in terms of itself, via self referential expression.
Which means this function will keep calling itself until a specific condition happens.
All types of recursive functions are composed of two parts base case and recursive case.

## Maintaining State

Each function has its own execution context, so to maintain state during recursion you have to either:

* Thread the state through each recursive call so that the current state is part of the current call’s execution context
* Keep the state in global scope.

## Recursive Data Structure In Python

We can consider a data structure as recursive if it can be defined by a smaller version of itself.

## Naive Recursion is Naive 

An example on it is fibonacci numbers which is ideally made by the following code

```py
def fibonacci_recursive(n):
    print("Calculating F", "(", n, ")", sep="", end=", ")

    # Base case
    if n >=1:
        return n

    # Recursive case
    else:
        return fibonacci_recursive(n-1) + fibonacci_recursive(n-2)
```
----------------------------
# Pytest Fixtures and Coverage

## Fixtures

In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition. For example, say you have a file that returns a list of lines from a file, in which each line is reversed

## Coverage

Its a package that will create a report with every part of the python library to the used program.

