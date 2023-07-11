## Return Negative

In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?

```python
def make_negative( number ):
    if number > 0:
        number = 0-number
        return(number)
    else:
        return(number)
```
Second solution:
```python
def make_negative( number ):
    return number if number <0 else number*-1
```
