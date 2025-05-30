# 19CS301Module-9
### EX: 9.1  MATRIX OPERATIONS

### Aim: To Write a Python Program to subtract two matrices by reading the matrix from the user.

### Algorithm: 
STEP 1: Start.
STEP 2: Create a variable r and c for rows and columns of the matrix.
STEP 3: Get the value of r and c from user.
STEP 4: Define a function to create a matrix.
STEP 5 : Define another function to subtract the matrices.
STEP 6: Print the result.
STEP 7 : Stop.

### Program:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
r,c=input().split()
A=create_matrix(int(r),int(c))
B=create_matrix(int(r),int(c))
C=[]
for i in range(int(r)):
    R=[]
    for j in range(int(c)):
        item=A[i][j]-B[i][j]
        R.append(item)
    C.append(R)
print(A)
print(B)
print(C)
```
### Output:
![image](https://github.com/user-attachments/assets/b1125b13-d26e-4404-acce-7dd2c1d2011c)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.2 LIST COMPREHENSION

### Aim: To Write a Python class program to generate all even numbers between 200 and 300 and store in a list using list comprehension.

### Algorithm:
STEP 1: Start.
STEP 2: Create a class.
STEP 3: Create variable a,b, and c for upper limit,lower limit and condition.
STEP 4: Intialise the values in the class.
STEP 5 : Define a method and using list comprehension calculate the result.
STEP 6: Print the result.
STEP 7 : Stop.

### Program:
```
class Generate:
    def __init__(self, first,d,last):
        self.first = first
        self.d = d
        self.last=last
    def Ap_generate(self):
        L=[i for i in range(self.first,self.last+1,self.d)]
        return L
Series = Generate(200,2,300)
print(Series.Ap_generate())

```
### Output:
 ![image](https://github.com/user-attachments/assets/a9707d46-2d47-4472-a6b3-b407a6f6ef71)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.3 ADVANCED LIST PROCESSING

### Aim: To Write a Python program to Find the transpose of a matrix using list Comprehension.

### Algorithm:

STEP 1: Start.
STEP 2: Create a variable r and c for rows and columns. 
STEP 3: Get the value of r and c from user.
STEP 4: Define a function to create the matrix.
STEP 5 : Using list comprehension find the transpose of the matrix.
STEP 6: Print the result.
STEP 7 : Stop.

### Program:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
    
r,c=input().split()
r=int(r)
c=int(c)
A=create_matrix(r,c)
print(A)
T = [[r[i] for r in A] for i in range(len(A[0]))]
print(T)

```
### Output:
![image](https://github.com/user-attachments/assets/411a227a-f44d-4b1a-b489-c7592dddbb67)

### Result: Thus, the given program is implemented and executed successfully .
 
### EX: 9.4 TOEPLITZ MATRIX

### Aim: To Write a Python Program to check whether the given matrix is Toeplitz Matrix.

### Algorithm:
STEP 1: Start.
STEP 2: Create a variable r and c for rows and columns.
STEP 3: Get the value of r and c from user.
STEP 4: Define a function to create the matrix.
STEP 5 : Using the formula check for TOEPLITZ MATRIX .
STEP 6: Print the result.
STEP 7 : Stop.

### Program:
```
def create_matrix(n,m):
    M=[]
    for i in range (n):
        row=[]
        for j in range (m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
def print_matrix(M):
    for i in range (len(M)):
        for j in range (len(M[0])):
            print(M[i][j],end=" ")
        print()
def isThoeplitz(M):
    for i in range (len(M)):
        for j in range (len(M[0])):
            if i>0 and j>0 and M[i][j]!=M[i-1][j-1]:
                return False
    return True
r,c=input().split()
A=create_matrix(int(r),int(c))
print("A=",A)
if isThoeplitz(A):
    print(A,"is a Toeplitz Matrix")
else:
    print(A,"is not a Toeplitz Matrix")
print_matrix(A)

```
### Output:

![image](https://github.com/user-attachments/assets/0fb8f81b-ab07-4b3e-b273-035a0f38566d)

### Result: Thus, the given program is implemented and executed successfully.
 
SEB-LIST COMPREHENSION

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

