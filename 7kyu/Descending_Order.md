## Descending Order
Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

Examples:<br>
Input: 42145 Output: 54421<br>
Input: 145263 Output: 654321<br>
Input: 123456789 Output: 987654321<br>

### Solution
```python
def descending_order(num):
    num_new=''
    num_list =[int(i) for i in str(num)]
    num_list.sort(reverse=True)
    for j in num_list:
        num_new += str(j)
    return int(num_new)
```
