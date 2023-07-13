## Abbreviate a Two Word Name

Write a function to convert a name into initials. This kata strictly takes two words with one space in between them.  
The output should be two capital letters with a dot separating them.
It should look like this:

```
Sam Harris => S.H
patrick feeney => P.F
```
### 1st method (split)
```python
def abbrev_name(name):
    return str((name.split(" ")[0][0]).upper() + "." + (name.split(" ")[1][0]).upper())
```
### 2nd method (split + join)
```python
def abbrev_name(name):
    words = name.split()
    initials = ".".join(word[0].upper() for word in words)
    return initials
```
