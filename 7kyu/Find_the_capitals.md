
## Find the capitals
Write a function that takes a single string (word) as argument. The function must return an ordered list containing the indexes of all capital letters in the string.
```
Example
Test.assertSimilar( capitals('CodEWaRs'), [0,3,4,6] );
```
### Solution
```python
def capitals(word):
    word_index = []
    x = 0
    for i in word:    
        if i.isupper():
            word_index.append(x)
        x += 1
    return word_index
```
