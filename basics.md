# Basics
NumPy is a powerful Python library for numerical operations. Some of its basic functions include:

1. **Arrays:** NumPy provides the `numpy.array` function to create arrays, which are multi-dimensional, homogeneous data structures.

   ```python
   import numpy as np

   arr = np.array([1, 2, 3])
   ```

2. **Array Operations:** NumPy allows element-wise operations on arrays, making it efficient for numerical computations.

   ```python
   a = np.array([1, 2, 3])
   b = np.array([4, 5, 6])

   result = a + b
   ```

3. **Mathematical Functions:** NumPy provides a wide range of mathematical functions that can be applied element-wise to arrays.

   ```python
   arr = np.array([1, 2, 3])

   square_root = np.sqrt(arr)
   ```

4. **Indexing and Slicing:** Similar to Python lists, NumPy arrays support indexing and slicing for accessing and modifying elements.

   ```python
   arr = np.array([1, 2, 3, 4, 5])

   sub_array = arr[1:4]
   ```

5. **Shape and Reshape:** NumPy provides functions to get the shape of an array and reshape it.

   ```python
   arr = np.array([[1, 2, 3], [4, 5, 6]])

   shape = arr.shape
   reshaped_arr = arr.reshape((3, 2))
   ```

6. **Linear Algebra Operations:** NumPy includes functions for linear algebra operations, such as matrix multiplication, eigenvalues, and solving linear systems.

   ```python
   matrix_a = np.array([[1, 2], [3, 4]])
   matrix_b = np.array([[5, 6], [7, 8]])

   product = np.dot(matrix_a, matrix_b)
   ```

These are just some of the basic functions of NumPy. It's a versatile library that forms the foundation for many scientific and data-related tasks in Python.

Certainly! NumPy provides a rich set of advanced functions for more complex and specialized operations. Here are some examples:

1. **Broadcasting:** NumPy allows operations between arrays of different shapes and sizes, through a feature called broadcasting. It automatically expands smaller arrays to match the shape of larger arrays.

   ```python
   a = np.array([[1, 2, 3], [4, 5, 6]])
   b = np.array([10, 20, 30])

   result = a + b  # Broadcasting the addition
   ```

2. **Universal Functions (ufuncs):** NumPy includes universal functions that operate element-wise on arrays, performing fast vectorized operations.

   ```python
   arr = np.array([1, 2, 3, 4])

   exp_arr = np.exp(arr)  # Element-wise exponentiation
   ```

3. **Aggregation Functions:** NumPy provides functions for aggregating data, such as `sum`, `mean`, `min`, `max`, and more. These functions can operate along specified axes.

   ```python
   matrix = np.array([[1, 2, 3], [4, 5, 6]])

   column_sum = np.sum(matrix, axis=0)
   ```

4. **Indexing with Boolean Arrays:** NumPy supports boolean indexing, allowing you to use boolean conditions to index and filter arrays.

   ```python
   arr = np.array([1, 2, 3, 4, 5])

   mask = arr > 2
   result = arr[mask]
   ```

5. **Random Number Generation:** NumPy includes a powerful random module for generating random numbers and samples from various probability distributions.

   ```python
   random_values = np.random.rand(3, 3)  # 3x3 array of random values between 0 and 1
   ```

6. **FFT (Fast Fourier Transform):** NumPy provides functions for fast and efficient FFT, which is essential for signal processing and frequency domain analysis.

   ```python
   signal = np.array([1, 2, 3, 4, 5])

   fft_result = np.fft.fft(signal)
   ```

7. **Memory Views:** NumPy allows creating memory views of arrays, which are alternative views of the same data without making a copy. This is useful for efficient memory usage.

   ```python
   arr = np.array([[1, 2, 3], [4, 5, 6]])

   memory_view = arr[:, ::2].T  # Creating a memory view
   ```

These advanced functions make NumPy a powerful library for scientific computing and data analysis in Python.
