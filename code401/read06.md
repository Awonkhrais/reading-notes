# How to use Random Module

* The random module provides access to functions that support many operations. 

## When to use it?

We want the computer to pick a random number in a given range Pick a random element from a list, pick a random card from a deck, flip a coin etc. When making your password database more secure or powering a random page feature of your website.

**Randint** : If we wanted a random integer, we can use the randint function Randint accepts two parameters: a lowest and a highest number.

```py
import random
print random.randint(0, 5)
This will output either 1, 2, 3, 4 or 5.
```

**Random** : If you want a larger number, you can multiply it.

```py
import random
random.random() * 100
```

**Choice** : Generate a random value from the sequence sequence.

```py
random.choice( ['red', 'black', 'green'] ).
The choice function can often be used for choosing a random element from a list.
```

```py
import random
myList = [2, 109, False, 10, "Lorem", 482, "Ipsum"]
random.choice(myList)
```

**Shuffle** : The shuffle function, shuffles the elements in list in place, so they are in a random order.

```py
from random import shuffle
x = [[i] for i in range(10)]
shuffle(x)
Output:
# print x  gives  [[9], [2], [7], [0], [4], [5], [3], [1], [8], [6]]
```
----------------------------------------------------

# What is Risk Analysis

* risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test. After that, the process of assigning the level of risk is done.

* Risk that you could encounter: 1. Use of new hardware, 2. Use of new tech, 3. Use of new automation tool, 4. The sequence of code, 5. availability of tests resources for the application.


## How to perform Risk Analysis?

1. Searching the risk
2. Analyzing the impact of each individual risk
3. Measures for the risk identified.