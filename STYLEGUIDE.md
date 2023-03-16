# Eagle Python Style Guide

### A lot of this style guide is based off the [Google Python Styleguide](https://google.github.io/styleguide/pyguide.html).


## Imports

### Standard Library Imports
#### stdlib libraries should be used with a general library-wide import.
##### ALLOWED
```py
import math
print(math.sqrt(2))
```
##### DISALLOWED
```py
from math import sqrt
print(sqrt(2))
```
### Third Party Imports
#### Third Party Libraries should be used with a function, or class wide import.
##### ALLOWED
```py
from numpy import sum
print(sum([2,2,4,6]))
```
##### DISALLOWED
```py
import numpy as np
print(np.sum([2,2,4,6]))
```


## Functions

### Function definitions
#### Functions should have an appropriate docstring.
##### ALLOWED
```py
def my_function():
    """
    This is a docstring.
    """
    return 0
```
##### DISALLOWED
```py
def my_function():
    return 0
```
#### Functions should have an appropriate type signature.
##### ALLOWED
```py
# function :: int -> int -> int
def function(x,y):
    return x * y
```
###### DISALLOWED
```py
def function(x,y):
    return x * y
```
