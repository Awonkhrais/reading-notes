# Dunder Methods

Dunder methods are special, predefined methods used to enrich classes. They are easy to recognize because they start and end with double underscores, for example __init__ or __str__. Broadly, they allow user-defined object types to emulate the behavior of built-in object types. This allows custom objects to return standard data such as length or a slice.

Object Initialization: __init__
The constructor takes care of setting up the object with various standardized properties


Object Representation: __repr__, __str__
__repr__: The “official” string representation of an object. The goal of __repr__ is to be unambiguous about an object instance's properties.

__str__: The “informal” or nicely printable string representation of an object intended for end user consumption.


Iteration: __len__, __getitem__, __reversed__

Operator Overloading for Merging Accounts: __add__

Callable Python Objects: __call__


# Statistics and Probability

Defining Probability:

At the most basic level, probability seeks to answer the question, “What is the chance of an event happening?” - where an event is some outcome of interest. The set of all possible events that can occur is called a sample space. By looking at the events that can occur, probability gives a framework for making predictions about how often events will happen.

Statistics apply mathematical methods to real world observations to determine how closely such observations match theoretical probability. For example, statistics could be used to measure how often a coin is likely to land on heads or tails.

Data Distributions:

A dataset subjected to statistical analysis is likely to comport to some probabalistic model which illustrates the relative probability of different events in the sample set occurring. The most important of these models is the normal distribution.