## Simple Pig Latin
Move the first letter of each word to the end of it, then add "ay" to the end of the word. Leave punctuation marks untouched.

Examples
```
pig_it('Pig latin is cool') # igPay atinlay siay oolcay
pig_it('Hello world !')     # elloHay orldway !
```

### Solution
```python
def pig_it(text):
    text2=''
    for i in text.split():
        text2 += i[1:]+i[0:1]
        if i not in ('!','?'):
            text2 += 'ay ' 
        else:
            text2 += ' ' 
    return text2[:-1]
```
