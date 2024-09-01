# ECE2112 - Advanced Computer Programming and Algorithms
## EXPERIMENT 2: NUMERICAL PYTHON (NUMPY)

### Custodio, Louise Angela G.
## 2ECE-D

**I. Intended Learning Outcomes**:
1. To identify the codes and functions incorporated in the Numpy library.
2. To be able to apply and use the different codes and functions in creating a Python program using a Numpy library.

**II. Instructions:**
Write a Python script/code in the Jupyter Notebook to do the given problems.

## Problems

**NORMALIZATION PROBLEM:** Normalization is one of the most basic preprocessing techniques in data analytics. This involves centering and scaling process. Centering means subtracting the data from the
mean and scaling means dividing with its standard deviation. Mathematically, normalization can be expressed as:

![Screenshot 2024-09-01 125839](https://github.com/user-attachments/assets/521de641-4e20-4b27-8fd6-f3181f5afa60)

In Python, element-wise mean and element-wise standard deviation can be obtained by using .mean() and .std() calls.
In this problem, create a random 5 x 5 ndarray and store it to variable X. Normalize X. 


**DIVISIBLE BY 3 PROBLEM:** Create the following 10 x 10 ndarray.

![Screenshot 2024-09-01 125846](https://github.com/user-attachments/assets/b9d9072a-c055-4761-ab72-e0f021fee87c)

which are the squares of the first 100 positive integers.
From this ndarray, determine all the elements that are divisible by 3.

## How I did my code:

### **NORMALIZATION PROBLEM**

![PA2-1](https://github.com/user-attachments/assets/dabd57ac-a2a7-453f-965e-f472e42f41ae)

Step 1: Create a 5x5 Matrix with Random Elements - I started by creating a 5x5 matrix with random values using 'np.random.random((5,5))'. This function generates values between 0 and 1 to populate the matrix.

Step 2: Print the Original Matrix
To display the original matrix, I printed the descriptive title "Original Array X:" followed by the matrix X itself. I added an empty 'print()' statement to insert a blank line for better readability between outputs.

Step 3: Calculate the Mean of the Matrix
I calculated the mean of matrix X by calling the '.mean()' function and stored the result in a variable named 'xbar'. This provides a single value representing the average of all elements in X.

Step 4: Print the Mean of the Matrix
I printed the text "Array X Mean: " followed by the value of 'xbar' to present the mean. 

Step 5: Calculate the Standard Deviation of the Matrix
I calculated the standard deviation using the '.std()' function, which measures the variability of the elements in X from the mean. The result was stored in the variable 'sd'.

Step 6: Normalize the Matrix
I normalized the matrix by subtracting the mean 'xbar' from each element in X and dividing the result by the standard deviation 'sd'. The normalized values were stored in a new matrix Z, standardizing the data for further analysis.

Step 7: Print the Normalized Matrix
I printed the title "Normalization of X:" to introduce the normalized data, followed by the contents of matrix Z.

### **DIVISIBLE BY 3 PROBLEM**

![PA2-2](https://github.com/user-attachments/assets/284ae5fa-5308-41ee-b23a-4c933104012e)

Step 1: Create and Square Elements in an Array - I began by creating a 1D NumPy array 'a' containing integers from 1 to 100. Each element in this array was squared using 'np.array(range(1,101))**2.'

Step 2: Resize the Array - I resized the 1D array 'a' into a 10x10 2D array using 'np.resize(a, (10,10)).' This transformed the array into a matrix with 10 rows and 10 columns, storing the result in variable 'A'.

Step 3: Print the Resized Matrix - I printed the title "A = " to label the output, followed by printing the contents of matrix 'A'. An empty 'print()' statement was added to insert a blank line for better readability between outputs.

Step 4: Identify Elements Divisible by 3 - To find elements in matrix 'A' that are divisible by 3, I used Boolean indexing: 'A[A%3==0].' This selects the elements where the condition is true, storing these elements in the variable 'div.'

Step 5: Resize the Array of Divisible Elements - I resized the array 'div' into a 3x11 matrix using 'np.resize(div, (3,11))', as there may be more elements than can fit into a 3x11 matrix, so the final shape might not fully represent all elements divisible by 3. The resized array was stored in the variable 'elem.'

## Conclusion

In this experiment, the Numpy library was explored through two key tasks, showcasing its functionalities and practical applications. The first task involved normalizing a 5x5 matrix by calculating its mean and standard deviation, illustrating how to standardize data for analysis. The second task required generating a 10x10 matrix of squared integers and identifying elements divisible by 3, highlighting the efficiency of Numpy’s array operations and indexing. These exercises provided valuable insights into data preprocessing and array manipulation, underscoring the importance of mastering Numpy for effective data analysis in Python.
