# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program and import the required library (numpy).
2.Initialize the matrix for which the LU decomposition needs to be found.
3.Apply LU Decomposition
4.Display the results

## Program:
/*
Program to find the L and U matrix.
Developed by: Nather Nabeel S A C
RegisterNumber: 212224100040
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

/*
Program to find the LU Decomposition of a matrix.
Developed by: Nather Nabeel S A C
RegisterNumber: 212224100040
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b= np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)


## Output:

<img width="1267" height="955" alt="image" src="https://github.com/user-attachments/assets/fb019b6c-d59b-4944-a04e-7de9ce4c1120" />

<img width="1306" height="872" alt="image" src="https://github.com/user-attachments/assets/b3abc7ae-3592-4974-8b71-2c85537f0b33" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

