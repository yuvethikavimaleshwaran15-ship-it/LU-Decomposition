# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
##5A)
step1  import numpy as np
step2 import the lu decomposition function (lu) using scipy.linalg
step3 read input from the user , convert into numpy array 
step4 perform PLU decompositionon matrix A
step5 print the element of lower triangular matrix
step6 print the element of upper triangular matrix.
##5B)
step1 import the numpy as np
step2 read input from the user for coefficient matrix A
step3 compute the LU decomposition of matrix a using lu_factor(a)
step4 solve and print the linear system using lu_solve((lu,p),b)

## Program:
##5a)
Developed by: Yuvethika V
RegisterNumber: 26016105
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu

A= np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
##5B)
Developed by: Yuvethika V
RegisterNumber: 26016105
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg  import lu_factor , lu_solve
a = np.array(eval(input()))
b = np.array(eval(input()))
lu,p=lu_factor(a)
x = lu_solve((lu,p),b)
print(x)
## Output:
##5A)
<img width="616" height="523" alt="image" src="https://github.com/user-attachments/assets/8a608698-6c6a-40f6-879c-f26f4588e8de" />
##5B)
<img width="432" height="377" alt="{DFEA0A9F-71F8-4479-9687-5D16A40B948A}" src="https://github.com/user-attachments/assets/e5bece78-9192-4df6-a760-c3c4dc91c850" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

