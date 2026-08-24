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
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: A.Ajayprabu
RegisterNumber: 212225220005
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*


# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)


*/
```

## Output:
<img width="1240" height="521" alt="image" src="https://github.com/user-attachments/assets/912de249-f344-4f62-abf5-d446cab91418" />

<img width="1260" height="277" alt="image" src="https://github.com/user-attachments/assets/712cbb4e-ae98-4587-a4b8-5ba645e117a9" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

