# Pandas 

pandas is a Python package providing fast, flexible, and expressive data structures designed to make working with “relational” or “labeled” data both easy and intuitive. It aims to be the fundamental high-level building block for doing practical, real world data analysis in Python.


How do you get pandas in my python project?

```
import numpy as np

import pandas as pd
```

* The two primary data structures of pandas :

1- Series (1-dimensional) ( 1D labeled homogeneously-typed array )

2- DataFrame (2-dimensional) ( General 2D labeled, size-mutable tabular structure with potentially heterogeneously-typed column )


```
To Reading data : `data = pd.read_csv('my_file.csv')`

To Writing data : `data.to_csv('my_new_file.csv', index=None)`
```