# In Tests We Trust - TDD with Python

* Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

* TDD stands for Test-Driven Development : is a strategy to think (and write!) tests first. (write a test before start coding)

AAA: Arrange, Act and Assert.

* Arrange: you need to organize the data needed to execute that piece of code (input)

* Act: here you will execute the code being tested (exercise the behaviour)

* Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

Note : Now you can execute the tests. I suggest the lib **pytest** to do it. But you are free to choose anything you like.

## The Cycle of TDD :

* The cycle is made by three steps:

1. Write a unit test and make it fail

2. Write the feature and make the test pass!

3. Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)


# If name equals main

If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 


# Recursion

Recursion : The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function.

* The idea is to represent a problem in terms of one or more smaller problems and a base condition to stop the recursion

* Direct vs Inderect - whether a function calls itself or another function

* tailed and non-tailed : A recursive function is tail recursive when recursive call is the last thing executed by the function.

![rec](https://media.geeksforgeeks.org/wp-content/cdn-uploads/Recursive-Functions-in-c.png)