# Game-A-Thon : Introduction to Git And Github
## Name : Ishita Khandekar
### Problem Statement 1 : Write a Python function that accepts a string and calculate the number of upper case letters and lower case letters.
#### TestCase 1 : Input : They spoke to him in French, but he responded in English.
#### Output : No. of Upper case characters :  3  
#### No. of Lower case Characters :  42

``` python
def string_test(s):
    d={"UPPER_CASE":0, "LOWER_CASE":0}
    for c in s:
        if c.isupper():
           d["UPPER_CASE"]+=1
        elif c.islower():
           d["LOWER_CASE"]+=1
        else:
           pass
    print ("Sentence : ", s)
    print ("No. of Upper case characters : ", d["UPPER_CASE"])
    print ("No. of Lower case Characters : ", d["LOWER_CASE"])

string_test('They spoke to him in French, but he responded in English.')
```

### Problem Statement 2 : Write a Python program to sort a list of elements using the insertion sort algorithm.
#### TestCase 2 : Input : [30,13,17,18,16,27,24,11,15,56,43,67,63]
#### Output : [11, 13, 15, 16, 17, 18, 24, 27, 30, 43, 56, 63, 67]

``` python
def insertionSort(nlist):
   for index in range(1,len(nlist)):

     currentvalue = nlist[index]
     position = index

     while position>0 and nlist[position-1]>currentvalue:
         nlist[position]=nlist[position-1]
         position = position-1

     nlist[position]=currentvalue

nlist = [30,13,17,18,16,27,24,11,15,56,43,67,63]
insertionSort(nlist)
print(nlist)
```
