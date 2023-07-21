

## Isograms

An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.

Example: (Input --> Output)
```
"Dermatoglyphics" --> true "aba" --> false "moOse" --> false (ignore letter case)

isIsogram "Dermatoglyphics" = true
isIsogram "moose" = false
isIsogram "aba" = false
```

### Solution #1 - set() function
```python
def is_isogram(string):
    string = string.lower()
    return(len(set(string)) == len(string)) #set() - to get unique values from list
```
### Solution #2
```python
def is_isogram(string):
    string = string.lower()
    for i in string:
        if string.count(i)>1:
            return False
    return True
```
