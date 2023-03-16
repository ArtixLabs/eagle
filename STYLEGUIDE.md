# Eagle Python Style Guide

### A lot of this style guide is based off the [Google Python Styleguide](https://google.github.io/styleguide/pyguide.html).


## Imports

* Standard Library Imports
  * stdlib libraries should be used with a general library-wide import.
    * ALLOWED
          import math
          print(math.sqrt(2))
    * DISALLOWED
          from math import sqrt
          print(sqrt(2))
* Third Party Imports
  * Third Party Libraries should be used with a function, or class wide import.
    * ALLOWED
          from numpy import sum
          print(sum([2,2,4,6]))
    * DISALLOWED
          import numpy as np
          print(np.sum([2,2,4,6]))



## Functions

* Function definitions
  * Functions should have an appropriate docstring.
    * ALLOWED
          def my_function():
              """
              This is a docstring.
              """
              return 0
    * DISALLOWED
          def my_function():
              return 0
  * Functions should have an appropriate type signature.
    * ALLOWED
          # function :: int -> int -> int
          def function(x,y):
              return x * y
    * DISALLOWED
          def function(x,y):
              return x * y
