## Get the Middle Character

You are going to be given a word. Your job is to return the middle character of the word. If the word's length is odd, return the middle character. If the word's length is even, return the middle 2 characters.

```python
def get_middle(s):
    s_len = len(s)
    index_middle =int((s_len-1)/2)
    if s_len >2:
        if s_len % 2 == 0:
            #middle 2 characters
            return (s[index_middle:-index_middle])
        else:
            #middle 1 character
            return (s[index_middle:-index_middle])
    else:
        return s
```
