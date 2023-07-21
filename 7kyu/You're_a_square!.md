## You're a square!

Write a function to convert a name into initials. This kata strictly takes two words with one space in between them.  
The output should be two capital letters with a dot separating them.
It should look like this:

```python
def is_square(n):
    if n>=0:
        if int(n**(1/2))**2 == n:
            return True
    return False
```

### Math
```python
import math
def is_square(n):
    sqrt_num = math.sqrt(n)
    if sqrt_num.is_integer():
        return True
    else:
        return False
```

