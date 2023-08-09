## Replace With Alphabet Position
Welcome.<br>

In this kata you are required to, given a string, replace every letter with its position in the alphabet.<br>

If anything in the text isn't a letter, ignore it and don't return it.<br>
```
"a" = 1, "b" = 2, etc.
```
Example<br>
`
alphabet_position("The sunset sets at twelve o' clock.")
Should return "20 8 5 19 21 14 19 5 20 19 5 20 19 1 20 20 23 5 12 22 5 15 3 12 15 3 11" ( as a string )
`
### Solution
```python
def alphabet_position(text):
    text = text.lower()
    new_text = ""
    for i in text:
        if i.isalpha():
            new_text += str(ord(i)-96)
            new_text += " "
    return new_text.rstrip()
```
