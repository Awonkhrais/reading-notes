# Readings: In memory storage

## Understanding the JavaScript Call Stack

![call](https://miro.medium.com/max/638/1*CCHexfHNCNo-f8aw3rbRew.jpeg)

1.What is a ‘call’?
A call is a function invocation, and a call stack is a hierarchy and ordering of these calls.

2.How many ‘calls’ can happen at once?
Calls in a call stack happen one at a time, from top to bottom.


3.What does LIFO mean?
LIFO means Last In, First Out data structure. It means that whichever one was most recently added, will be the first one to leave the stack when the function returns.

What causes a Stack Overflow?

A stack overflow will occur when there is a recursive function, or a function that calls itself. When a function is added onto the stack many times, the browser will accomodate what it can hold, but eventually it will throw an error saying that the stack is over filled.

## JavaScript error messages

What is a ‘syntax error’?
A syntax error is like the grammatical errors you have when writing sentences. It is when the language cannot parse the code you have written - "in terms of syntax"

What is a ‘range error’?
A range error occurs if you are using a range for any of your code, and the range is invalid.

What is a ‘type error’?
A type error essentially is if you can not access the data type you are trying to access

What is a breakpoint?
a break point is a point in which your code will stop running, and allow you to check the values at that point.

What does the word ‘debugger’ do in your code?
The word debugger in JavaScript will stop the execution of your code and call a debugger function.