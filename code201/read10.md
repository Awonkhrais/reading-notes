# Debugging

- to learn how to solve programming errors we should know about :
1. THE CONSOLE & DEV TOOLS
     - Tools built into the browser
that help you hunt for errors. 
2. COMMON PROBLEMS
    - Common sources of errors,
and how to solve them.
3. HANDLING ERRORS
    - How code can deal with potential errors gracefully. 


### ORDER OF EXECUTION :
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.
![ORDER OF EXECUTION](https://blog.risingstack.com/content/images/2019/01/Execution_timing_event_loop_with_microtask_queue.svg)

### EXECUTION CONTEXTS
The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope. 

### THE STACK
 The JavaScript interpreter processes one line of code at a time. When a statement needs data from another function, it stacks (or piles) the new function on top of the current task.

 ### EXECUTION CONTEXT & HOISTING
 Each time a script enters a new execution context, there are two phases
of activity: 

1. PREPARE

-  The new scope is created

-  Variables, functions, and arguments are created

- The value of the this keyword is determined

2. EXECUTE
- Now it can assign values to variables
- Reference functions and run their code
- Execute statements 

### ERROR OBJECTS:
Error objects can help you find where your mistakes are
and browsers have tools to help you read them. 

When an Er ror object is created, it will contain the
following properties:
- PROPERTY DESCRIPTION
- name Type of execution
- message Description
- file eNumber Name of the JavaScript file
- line neNumber Line number of error 

![ERROR OBJECTS](https://i.stack.imgur.com/QnUPb.png)

### Error object types:
- Eval Error

INCORRECT USE OF eval() FUNCTION
The eval () function evaluates text through the
interpreter and runs it as code.

- URI Error

INCORRECT USE OF URI FUNCTIONS
If these characters are not escaped in URls, they will
cause an error: / ? & I : ;

- Type Error

VALUE IS UNEXPECTED DATA TYPE
This is often caused by trying to use an object or
method that does not exist. 

- RangeError
NUMBER OUTSIDE OF RANGE
If you call a function using numbers outside of its
accepted range. 

**Note**:

NaN
NOT AN ERROR! If you perform a mathematical operation using
a value that is not a number, you end up with the
value of NaN, not a type error.
NOT A NUMBER



