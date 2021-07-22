# Python NumPy
## Introduction
### NumPy vs List
* NumPy is faster because it has a fixed type and it uses less bytes of memory
* We don't need to do type checking when using NumPy
* NumPy utilizes contiguous memory
    * SIMD(Single Instruction Multiple Data) Vector Processing
    * Effective Cache Utilization
## Syntax
### Array
* 1D array: `np.array([1,2,3])`
* possible for two numpy arraies to multiple each other
* 2D array: `np.array([9.0,8.0],[7.0,6.0])`
* Get Dimension
    * `(array name).ndim`
* Get Shape
    * `(array name).shape`
* Get Type
    * `(array name).dtype`
* Get Size / total size
    * `(array name).itemsize`
    * `(array name).size` or `(array name).nbytes` 
### Access and Change
* Get a specific element
    * `(array name)[row index, column index]`
* Get a specific row
    * `(array name)[row index, :]`
* Slice
    `[start index, end index, step size]`
* Be caredul when copying arrays
### Linear Algebra
* Multiple of matrixes
    * `np.matmul(array1,array2)`
    