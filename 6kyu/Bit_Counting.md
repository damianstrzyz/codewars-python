## Bit Counting
Write a function that takes an integer as input, and returns the number of bits that are equal to one in the binary representation of that number. You can guarantee that input is non-negative.

The binary representation of `1234` is `10011010010`, so the function should return `5` in this case

---
### Solution 1
```python
def count_bits(n):
    x=0
    for i in bin(n):
        if i=="1":
            x=x+1
    return x
```
---
### Solution 2
```python
return bin(n).count("1")
```
