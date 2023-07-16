## Get the Middle Character

You are going to be given a word. Your job is to return the middle character of the word. If the word's length is odd, return the middle character. If the word's length is even, return the middle 2 characters.

```python
def get_middle(s):
    s_len = len(s)
    i =int((s_len-1)//2)
    if s_len >2:
        if s_len % 2 == 0:
            #middle 2 characters
            return (s[i:-i])
        else:
            #middle 1 character
            return (s[i:-i])
    else:
        return s
```
Optimization:
```python
def get_middle(s):
    i =(len(s)-1)//2
    return(s[i:-i]) or s
```
