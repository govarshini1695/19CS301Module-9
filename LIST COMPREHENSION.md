LIST COMPREHENSION

AIM:
To write a python program to store a scalar multiple of a set of numbers  in a list using list
comprehension.

ALGORITHM:
STEP 1:Start the program.
STEP 2:Define a list containing a set of numbers.
STEP 3:Take input for a scalar value.
STEP 4:Use list comprehension to multiply each number in the list by the scalar value and store
the results in a new list.
STEP 5:Return or print the newly created list.
STEP 6:End


PROGRAM:

```
n=int(input())
scl=int(input())
l=[]
for i in range(n):
    x=float(input())
    l.append(x)
sq_l=[item*scl for item in l]
print(l)
print(sq_l)
```

OUTPUT:

![image](https://github.com/user-attachments/assets/c0e9d278-9057-4c54-a439-4e64fdeeeeb0)


RESULT: Thus the python program to store a scalar multiple of a set of numbers  in a list using
list comprehension. 
