
## Shortest Word

Simple, given a string of words, return the length of the shortest word(s).

String will never be empty and you do not need to account for different data types.

```python
def find_short(s):
    list = []
    for i in s.split():
        list.append(len(i))
    return(min(list))
```
