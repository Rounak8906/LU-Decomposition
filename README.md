# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1 :Start the program and import the required libraries (NumPy and SciPy).
### Step 2 :Define the matrix using NumPy.
### Step 3 :Use lu() to perform LU decomposition and display the lower and upper triangular matrices.
### Step 4 :Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.
### Step 5 :Display the solution and end the program.

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: 
RegisterNumber: 
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]= "1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: 
RegisterNumber: 
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),B)
print(X)
```

## Output:
<img width="1217" height="453" alt="image" src="https://github.com/user-attachments/assets/960c5ca4-e7c2-40b7-9344-9c5dc14de913" />
<img width="1212" height="766" alt="image" src="https://github.com/user-attachments/assets/1bb8e32a-e1c9-46ed-b3b6-8438af94c892" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

