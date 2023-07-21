## Complementary DNA
Deoxyribonucleic acid (DNA) is a chemical found in the nucleus of cells and carries the "instructions" for the development and functioning of living organisms.

If you want to know more: http://en.wikipedia.org/wiki/DNA

In DNA strings, symbols "A" and "T" are complements of each other, as "C" and "G". Your function receives one side of the DNA (string, except for Haskell); you need to return the other complementary side. DNA strand is never empty or there is no DNA at all (again, except for Haskell).

More similar exercise are found here: http://rosalind.info/problems/list-view/ (source)

Example: (input --> output)
```
"ATTGC" --> "TAACG"
"GTAT" --> "CATA"
```
### Solution
```python
def DNA_strand(dna):
    dna2 =''
    for i in dna:
        if i == 'A':  
            dna2+='T' #or dna2+=(i.replace('A', 'T'))
        if i == 'T': 
            dna2+='A' #or dna2+=(i.replace('T', 'A'))
        if i == 'G': 
            dna2+='C' #or dna2+=(i.replace('G', 'C'))
        if i == 'C': 
            dna2+='G' #or dna2+=(i.replace('C', 'G'))
    return dna2
```
