# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program
 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: keerthana k
RegisterNumber: 212225230137
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: keerthana k
RegisterNumber: 212225230137
*/

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array([[3, 2, 7], [2, 3, 1], [3, 4, 1]])
b = np.array([4, 5, 7])
lu, piv = lu_factor(A)
x=lu_solve((lu, piv),b)
print(x)
```
## Output:
<img width="1257" height="802" alt="Screenshot 2026-03-23 110200" src="https://github.com/user-attachments/assets/44ee3ca1-b3e6-4533-95c1-23d292117765" />
<img width="1246" height="625" alt="Screenshot 2026-03-23 110212" src="https://github.com/user-attachments/assets/b05fdbad-ab54-4e01-9afa-e909d4fd3083" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

