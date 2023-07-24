## Break camelCase
Complete the solution so that the function will break up camel casing, using a space between words.
```
Example
"camelCasing"  =>  "camel Casing"
"identifier"   =>  "identifier"
""             =>  ""
```
### Solution 1
```python
def solution(s):
    for i in s:
        if i.isupper():
            s=s.replace(i,(" "+i)).replace("  "," ")
    return s
```
