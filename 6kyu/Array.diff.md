## Array.diff
Complete the solution so that the function will break up camel casing, using a space between words.<br>
Your goal in this kata is to implement a difference function, which subtracts one list from another and returns the result.<br>
It should remove all values from list a, which are present in list b keeping their order.
```
array_diff([1,2],[1]) == [2]
```
If a value is present in b, all of its occurrences must be removed from the other:
```
array_diff([1,2,2,2,3],[2]) == [1,3]
```
### Solution
def array_diff(a, b):
    c=[]
    for i in a:
        if i not in b:
            c.append(i)
    return c
```
