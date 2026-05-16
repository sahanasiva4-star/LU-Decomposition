# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
~~~
1.Import the necessary libraries(numpy,scipy.linalg) to use the built-in functions for calculation
2.Prepare the lists from each linear equations and assign in np.array()
3.Using the lu(), lu_solve(), lu_factor(), we can find the solutions.
4.End the program
~~~


## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: SAHANA S
RegisterNumber: 212225230236
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p, l, u = lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: SAHANA S
RegisterNumber: 212225230236
'''
# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu, pivot=lu_factor(a)
x=lu_solve((lu,pivot), b)
print(x)
```

## Output:
<img width="1163" height="420" alt="image" src="https://github.com/user-attachments/assets/812e9b91-ff46-4bc4-be38-fbe95d3d5ac7" />
<img width="996" height="174" alt="image" src="https://github.com/user-attachments/assets/7e9e806e-28a7-4687-b43a-2d39f746d9cc" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

