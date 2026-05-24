# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required library (numpy).
2. Initialize the matrix for which the LU decomposition needs to be found.
3. Apply LU Decomposition
4. Display the results

## Program:
(i) To find the L and U matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
```

## Output:
<img width="1920" height="931" alt="Screenshot 2026-05-24 151853" src="https://github.com/user-attachments/assets/f7e3ba4b-d442-4936-ad29-d9008521449c" />

<img width="1897" height="925" alt="Screenshot 2026-05-24 151947" src="https://github.com/user-attachments/assets/17edb1af-d2c7-4224-9b8a-372f75a1cdaf" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

