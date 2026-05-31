# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Jesu Joyal J
RegisterNumber: 212225040154
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np 
from scipy.linalg import lu
A = eval(input())
A = np.array(A, dtype=float)
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Jesu Joyal J
RegisterNumber: 212225040154
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = eval(input())
B=eval(input())
A = np.array(A,dtype=float)
b = np.array(B,dtype=float)
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
```

## Output:

<img width="1213" height="843" alt="image" src="https://github.com/user-attachments/assets/260d8765-c144-4b79-92db-f0fb368240fc" />

<img width="1091" height="893" alt="image" src="https://github.com/user-attachments/assets/2b9f94ce-66cb-4f94-8aba-4e3f7d33aeca" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

