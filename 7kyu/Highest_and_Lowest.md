## Highest and Lowest
In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.<br>

Examples<br>
high_and_low("1 2 3 4 5")  # return "5 1"<br>
high_and_low("1 2 -3 4 5") # return "5 -3"<br>
high_and_low("1 9 3 4 -5") # return "9 -5"<br>
Notes<br>
All numbers are valid Int32, no need to validate them.
There will always be at least one number in the input string.<br>
Output string must be two numbers separated by a single space, and highest number is first.<br>

```python
def high_and_low(numbers: list): #change to list
    numbers_new = [int(i) for i in numbers.split()]  #converting all strings in list to integers
    return " ".join([str(max(numbers_new)),str(min(numbers_new))])
```
