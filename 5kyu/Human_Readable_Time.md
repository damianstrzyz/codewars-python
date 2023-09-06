## Human Readable Time
Write a function, which takes a non-negative integer (seconds) as input and returns the time in a human-readable format (HH:MM:SS)
```
HH = hours, padded to 2 digits, range: 00 - 99
MM = minutes, padded to 2 digits, range: 00 - 59
SS = seconds, padded to 2 digits, range: 00 - 59
```
The maximum time never exceeds 359999 (99:59:59)

You can find some examples in the test fixtures.
### Solution
```python
def make_readable(seconds):
    h=0
    m=0
    s=0

    if seconds>=3600:
        h =int(seconds/3600)
    if seconds-(h*3600)>=60:
        m =int((seconds-(h*3600))/60)   
    if seconds-(m*60)>1:
        s=int((seconds-(h*3600))-m*60)  

    if s<10:
        s= "0"+str(s)
    if int(m)<10:
        m= "0"+str(m)    
    if int(h)<10:
        h= "0"+str(h)

    return (str(h)+':'+str(m)+':'+str(s))
```
