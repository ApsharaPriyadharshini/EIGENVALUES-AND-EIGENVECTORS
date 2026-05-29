# EIGENVALUES-AND-EIGENVECTORS
## Aim:
To write a python program to find the Eigenvalues and Eigen Vectors
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 : Import required libraries
### Step 2: Create the matrix using NumPy array
### Step 3: Using the np.linalg.eig(),  we get two results (first is eigenvalue and second is eigenvector) of the given matrix.
### Step 4: Sort eigenvalues and eigenvectors

## Program:
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np


A = np.array([[2, 2],
              [1, 3]])

eig_vals, eig_vecs = np.linalg.eig(A)


idx = np.argsort(eig_vals)
eig_vals = eig_vals[idx]
eig_vecs = eig_vecs[:, idx]


print("Eigen values are", eig_vals, "and Eigen Vectors are", eig_vecs)
## Output:
<img width="1274" height="336" alt="image" src="https://github.com/user-attachments/assets/47ed7571-e295-4ff0-b9a8-b8de13b82bef" />
<img width="1280" height="322" alt="image" src="https://github.com/user-attachments/assets/16a3d082-22f4-46e5-b18a-dfed9fa0f15e" />


## Result:
Thus the Eigenvalue and Eigenvector is successfully solved using python program
