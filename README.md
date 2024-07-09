# NumPy
For learning purpose


**What is NumPy?**
* Numpy is a multi-dimensional array library
* We can store 1D, 2D, 3D,.... upto N-Dimensional arrays
       
**How are Lists diferent from NumPy?**
* Lets say we have a (3X4) metrix with all integer values => [[3, 1, 2, 4],[5, 7, 1, 2][4, 1, 0, 1]]
* lets take 5 from the metrix and see how it is stored in the numpy array and lists

* In numpy 5 ==> 00000101(Binary) ==> 00000000 00000000 00000000 00000101(Int32)

* In Lists 5==> 00000101 ==> Need lot more information to store this integer

(Lists uses built-in int type it consists of 4 things
*Size:- Size of the integer value
*Reference Count:- How many times that integer is being pointed at
*Object Type:-
*Object Value:- it has its own bits assosiated with it
In Lists 5 ==> **00000000 00000000 00000000 00011100(Size)
               00000001 00111101 11111110 10111100 00011010 11011101 10100100 11011000(Reference Count)
               11001010 10111110 01100001 01000100 11111100 00000000 11001100 01011111(Object Type)
               00000000 00000000 00000000 00000000 00000000 00000000 00000000 00000101(Object Value)**)
               
**Benefits of Contiguous Memory**
-> SIMD Vector Processing
-> Effective Cache Utilization

**Lists**
* Lists are slower because its takes lot more space than numpy
->Each element has to be type checked while iterating through it
->Lists doesnt ustilize Contiguous memory
->The list is actually containing pointer to the actual information scattered around the computer memory
-> Operations that can be performed:- Insertion, deletion, appending, concatination, etc.

**NumPy**
->NumPy is faster than lists because numpy uses fixed types
->NumPy doesn't requires type checking
->Numpy utilizes Contiguous Memory
->All the elements of the array are stored next to each other in the computer memory
->Operations that can be performed:- Insertion, deletion, appending, concatination, etc. and lots more

**Application of NumPy?**
Mathematics (MATLAB Replacement)
Plotting (Matplolib)
Backend (Pandas, Connect4, Digital Photography)
Machine Learning
