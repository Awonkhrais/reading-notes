# Python Scope

* The concept of scope rules how variable and names are looked up in your code. It determines the visibility of a variable within the code.

* LEGB - stands for Local, Enclosing, Global and Built-in

* Global scope: The names that you define in this scope are available to all your code.

* Local scope: names that you define are only available or visible to the code within the scope.

## The Global Scope

* From the moment you start a Python program, you're in the global scope. Internally, Python turns your program's main script into a module called main to hold the main program's execution.

* Module Scope and global scope are the same since global scope/names are tightly associated with modules files and top-level names in any Python module.

* Whenever you run a Python program, the interpreter exectuest the code in the module or script that serves as an entry point to your program. This module is loaded with the specail name, main. Fromt this point on, you can say that your main global scope is the scope of main.

## The Enclosing Scope

* Enclosing or nonlocal scope is observed when you nest functions inside other functions.

* Names that you define in the enclosing Python scope are known as nonlocal names.

* When you call outer_func(), you’re also creating a local scope. The local scope of outer_func() is, at the same time, the enclosing scope of inner_func(). From inside inner_func(), this scope is neither the global scope nor the local scope. It’s a special scope that lies in between those two scopes and is known as the enclosing scope.