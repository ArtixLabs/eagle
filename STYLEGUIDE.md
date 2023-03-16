# Eagle Python Style Guide

### A lot of this style guide is based off the [Google Python Styleguide](https://google.github.io/styleguide/pyguide.html).


## Imports

### Standard Library Imports
#### STDLIB LIBRARIES SHOULD BE USED WITH A GENERAL LIBRARY-WIDE IMPORT.
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
#### THIRD PARTY LIBRARIES SHOULD BE USED WITH A FUNCTION, OR CLASS WIDE IMPORT.
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
#### FUNCTIONS SHOULD HAVE AN APPROPRIATE DOCSTRING.
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
#### FUNCTIONS SHOULD HAVE AN APPROPRIATE TYPE SIGNATURE.
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
