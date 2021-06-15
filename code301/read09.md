# Readings: FUNCTIONAL PROGRAMMING

# *Functional Programming Concepts*
- What is functional programming?
  - A design structure that focuses on mathmatical functions and avoids changing state or other mutable data.
- What is a pure function and how do we know if something is a pure function?
  - A pure function always gives the same outputs with the same inputs. Also it does noto cause any other observable effects on the state of the program.
- What are the benefits of a pure function?
  - The ease with which we can test the function using automated tools because no randomness needs to be accounted for.
- What is immutability?
  - It means that the state of something with this property can not be changed. To alter it you need to create a new object.
- What is Referential transparency?
  - It is something that we for sure know the output of. When immutable data is worked through a pure function we will always know what the output will be making it have referential transparency.

# *Node JS: Modules and Require*
- What is a module?
  - A bit of code with certain functionality that can solve a problem for the larger program. 
- What does the word ‘require’ do?
  - Require takes a string that is a path to the module you want to import and brings in the module located there.
- How do we bring another module into the file the we are working in?
  - Use require('file_pathway')  to find the module.
- What do we have to do to make a module available?
  - Use module.exports = function_Name
