## Exes and Ohs

Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.

Examples input/output:
```
XO("ooxx") => true
XO("xooxx") => false
XO("ooxXm") => true
XO("zpzpzpp") => true // when no 'x' and 'o' is present should return true
XO("zzoo") => false
```
## Solution #1
```python
def xo(s):
    s=s.lower()
    o_sum = 0
    x_sum = 0
    for i in s:
        if i == "o":
            o_sum = o_sum +1
        if i == "x":
            x_sum = x_sum +1
    if x_sum==o_sum:
        return True
    else:
        return False
```
## Solution #2 - count() function
```python
def xo(s):
    o_sum = s.lower().count('o')
    x_sum = s.lower().count('x')
    
    if o_sum == x_sum:
        return True
    else:
        return False
```
