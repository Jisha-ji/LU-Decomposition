# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i) To find the L and U matrix

1. Start
2. Import numpy as np and lu from scipy.linalg.
3. Input matrix A from the user.
4. Convert the input to a NumPy array.
5. Perform LU decomposition using lu(A)
→ Get matrices P, L, and U.
6. Print the L (Lower triangular) matrix.
7. Print the U (Upper triangular) matrix.
8. End

(ii) To find the LU Decomposition of a matrix

1. Start
2. Import numpy as np and lu_factor, lu_solve from scipy.linalg.
3. Input matrix A and vector b from the user.
4. Convert inputs to NumPy arrays.
5. Compute LU decomposition of A using lu_factor(A)
→ Get lu and piv.
6. Solve the system Ax = b using lu_solve((lu, piv), b)
→ Store result in X.
7. Print the solution vector X.
8. End

## Program:
(i) To find the L and U matrix
```
Program to find the L and U matrix.
Developed by: Jisha Bossne SJ
RegisterNumber: 212224230106
```
```
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
Program to find the LU Decomposition of a matrix.
Developed by: Jisha Bossne SJ
RegisterNumber: 212224230106
```
```
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```
## Output:

![Screenshot 2025-04-17 084246](https://github.com/user-attachments/assets/58368442-837e-4c25-80b9-aa29b91ca41b)
![Screenshot 2025-04-17 084309](https://github.com/user-attachments/assets/f0e7a618-e4a9-47fb-9abd-083504db4a8b)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

