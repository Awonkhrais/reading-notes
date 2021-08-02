# List Comprehensions

List comprehensions provide a concise way to create lists.

It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.

```py
new_list = [expression(i) for i in old_list if filter(i)]
```
This is equivalent to:

```py
for item in list:
    if conditional:
        expression
```

Example:

```py
listOfWords = ["this","is","a","list","of","words"]

items = [ word[0] for word in listOfWords ]

print items
The output should be: [‘t’, ‘i’, ‘a’, ‘l’, ‘o’, ‘w’]
```