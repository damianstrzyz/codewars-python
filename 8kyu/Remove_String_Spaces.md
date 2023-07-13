## Remove String Spaces

Write a function that removes the spaces from the string, then return the resultant string.

Example:
```
Input -> Output
"a b c" -> "abc"
```

### 1st method (replace)
```python
def no_space(x):
    return x.replace(" ", "")
```

### 2nd method (split and join)
```python
def no_space(x):
    return "".join(x.split())
```

### 3rd method (loop)
```python
def no_space(x):
    y = ""
    for i in x:
        if i != " ":
            y += i
    return y
```
