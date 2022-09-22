# pymatops - A Python package for Matrix Operations


[![Package Status](https://img.shields.io/badge/pypi-1.3.0-blue)](https://pypi.org/project/pymatops/)
[![Package Status](https://img.shields.io/badge/status-stable-brightgreen)](https://pypi.org/project/pandas/)

## Package Details
The <b> *pymatops* </b> package is [available](https://pypi.org/project/pymatops/) on the official Python Package Index (PyPi) repository.
It can be installed and used in your projects by running the following command using `pip`
```sh
pip install pymatops
```

## Package Operations
### 1. visualize - visualize a matrix
```python
import pymatops as pmo
mat = [[1,2,3], [4,5,6], [7,8,9]]
pmo.visualize(mat)
```
   
![image](https://user-images.githubusercontent.com/71393551/189523937-663903d9-fa9a-4577-9ccb-20a536121410.png)
 ---  
### 2. dim - returns a tuple with the dimensions of the matrix
```python
import pymatops as pmo
mat = [[1,2,3], [4,5,6], [7,8,9]]
print("The dimension of the matrix is ", pmo.dim(mat))
```
   
![image](https://user-images.githubusercontent.com/71393551/189525289-eb6aac0d-6a2c-4f8a-9b49-942eb01164b3.png)
---

### 3. randomMatrix - returns a matrix of random dimensions with random values if the function is called with no arguments
```python
import pymatops as pmo
print("The randomly generated matrix: ")
pmo.randomMatrix()
```
   
![image](https://user-images.githubusercontent.com/71393551/189525444-5258403a-63a9-4888-9141-5876c22d1534.png)
---

### 4. randomMatrix - you can pass dimensions to get a matrix of specified dimensions with random values. Both row and col dimensions are required
```python
import pymatops as pmo
print("The random matrix of dimension 6*8 generated: ")
pmo.randomMatrix(6,8)
```
   
![image](https://user-images.githubusercontent.com/71393551/189525132-b32781b2-4555-4747-9c0d-1938fd2a0ba4.png)
---

### 5. matSum - returns the sum of all elements in the matrix passed
```python
import pymatops as pmo
print("The random matrix generated: ")
mat = pmo.randomMatrix(6,8) # retuns a 6*8 matrix with random values
print("The sum of the matrix: ", pmo.matSum(mat))
```
   
![image](https://user-images.githubusercontent.com/71393551/189525090-9d39c9b2-d66d-4e0e-a1db-93949befa21f.png)
---

### 6. matAdd - returns the resultant matrix of the sum of matrix A and B
```python
import pymatops as pmo
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
mat1 =[[1, 2, 3], [4, 5, 6], [7, 8, 9]] # returns a 6*8 matrix with random values
print("Matrix 1:")
pmo.visualize(mat)
print("Matrix 2:")
pmo.visualize(mat1)
print("The resultant matrix of the matrix addition operation: ")
pmo.matAdd(mat, mat1)
```
   
![image](https://user-images.githubusercontent.com/71393551/189525607-1728f769-3d66-4671-a471-dfd08163c2a0.png)
---

### 7. matMul - returns the resultant matrix of the multiplication of matrix A and B
```python
import pymatops as pmo
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]] # matrix of dimensions 4*3
mat1 =[[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]] # matrix of dimensions 3*4
print("Matrix 1:")
pmo.visualize(mat)
print("Matrix 2:")
pmo.visualize(mat1)
print("The resultant matrix of the matrix multiplication operation: ")
pmo.matMul(mat, mat1)
```

![image](https://user-images.githubusercontent.com/71393551/189525779-520f9c71-5465-4a79-b87b-517e37c36f25.png)
---

### 8. scalarMul - returns the resultant matrix of the multiplication of matrix A with scalar c
```python
import pymatops as pmo
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print("Original Matrix: ")
pmo.visualize(mat)
print("Matrix after scalar multiplication operation: ")
pmo.scalarMul(mat, 3)
```

![image](https://user-images.githubusercontent.com/71393551/189524660-e03a5a87-6784-4cda-9261-9961d4ee9076.png)
---

### 9. transpose - returns transpose of matrix
```python
import pymatops as pmo
mat = [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]]
print("Original Matrix: ")
pmo.visualize(mat)
print("Matrix after transpose operation: ")
pmo.transpose(mat)
```

![image](https://user-images.githubusercontent.com/71393551/189524731-c00b8a62-650c-4447-9b63-08fc034cf657.png)
---

### 10. zeroElements - returns the number of zero elements in the matrix
```python
import pymatops as pmo
mat = [[1, 0, 3], [0, 5, 6], [7, 8, 0], [10, 11, 12]]
print("Original Matrix: ")
pmo.visualize(mat)
print("Number of zeros in the matrix: ", end = " ")
print(pmo.zeroElements(mat))
```

![image](https://user-images.githubusercontent.com/71393551/189524851-7b7342e5-1eff-493c-820c-0b9882abe3b6.png)
---

### 11. evenCheck - returns a tuple with the first element as the number of even numbers in the matrix and the second element being the number of odd numbers in the matrix
```python
import pymatops as pmo
mat = [[1, 0, 3], [0, 5, 6], [7, 8, 0], [10, 11, 12]]
print("Original Matrix: ")
pmo.visualize(mat)
print("Number of even numbers in the matrix: ", end = " ")
print(pmo.evenCheck(mat)[0])
print("Number of odd numbers in the matrix: ", end = " ")
print(pmo.evenCheck(mat)[1])
```

![image](https://user-images.githubusercontent.com/71393551/189524919-aed32588-6b9c-415e-a58a-33d7e5622813.png)
---

<div align="center">
   <b>Developed by Yash Seth (c) 2022</b>
</div>