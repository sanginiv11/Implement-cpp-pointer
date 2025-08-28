# Implementation of Basics of Pointers in C++  

### **Objective**  
To explore and practice the fundamental concepts of pointers in C++.  

**Software Used:** MinGW Compiler, Visual Studio Code, Online C++ compiler  

***

## **Program 1: Different ways to display pointer output**  
### Explanation and Theory  
This program introduces how pointers represent memory addresses in C++. An integer `a` is declared and a pointer stores its address. The code then prints:  
- the value of `a`,  
- the address of `a` using `&a`,  
- the pointer variable `p` (which holds the address) and,  
- the dereferenced pointer value `*p`, which retrieves the stored data.  

This demonstrates how variables are linked with their addresses and how dereferencing helps access contents stored at those addresses.  

### Algorithm  
1. Start  
2. Declare an integer `a` and store a value in it  
3. Create a pointer `p` and assign the address of `a`  
4. Print value of `a`  
5. Print address of `a` using `&a`  
6. Print the pointer `p` (address stored)  
7. Print the dereferenced value `*p`  
8. Stop  

***

## **Program 2: Changing variable value using a pointer**  
### Explanation and Theory  
This program highlights how pointers allow variable modification. An integer `a` is created, and a pointer stores its address. By dereferencing the pointer, the program first prints the original value. The value is then updated through `*p = new_value`, which directly changes `a`. Additionally, the program shows pointer-array relation by printing the first element of an array using both `*array` and `array`, validating their equivalence.

### Algorithm  
1. Start  
2. Initialize integer `a` with a value  
3. Create a pointer `p` assigned to `&a`  
4. Print value using `*p`  
5. Modify the stored value through pointer `*p = new_value`  
6. Print updated value of `a`  
7. Declare an integer array of size 5  
8. Print first element using `*array`  
9. Stop  

***

## **Program 3: Pointer incrementation (Pointer arithmetic)**  
### Explanation and Theory  
This program demonstrates how pointers interact with arrays via arithmetic operations. An array of five integers is declared, and a pointer `p` points to its first element. Initially, the program prints the value of the first element. Then, inside a loop, the pointer is incremented (`p++`), which shifts it to the next element in memory, allowing consecutive access to all array entries. This reflects how pointers and arrays are tightly coupled in C++ for sequential memory navigation.  

### Algorithm  
1. Start  
2. Declare an array `a = {10,20,30,40,50}`[5]
3. Assign pointer `p = a` (base address of array)  
4. Print value pointed by `p` (first element)  
5. Loop through array elements:  
   - Print `*p`  
   - Increment pointer `p++`  
6. Stop  

***

## **Program 4: Understanding call by value with pointers**  
### Explanation and Theory  
This experiment differentiates between passing parameters normally (call by value) and using pointers. A function is created to swap numbers, but when values are given directly, only **local copies** are changed. The original variables in `main()` remain the same. This makes clear that in call by value, modifications inside functions don’t affect real arguments.  

### Algorithm  
1. Start  
2. Define a function `swap(x, y)` using temporary variable for exchange  
3. Call function with variables from `main()`  
4. Print swapped values inside function  
5. Print original values in `main()` (unchanged)  
6. Stop  

***

## **Program 5: Call by address (using pointers for updation)**  
### Explanation and Theory  
This program shows **how pointers enable direct changes in original data**. A function receives addresses of two integers and swaps them using dereferenced pointers. Since the memory itself is accessed, updates are reflected back in `main()`. In addition, another version demonstrates increment: when an integer is passed by reference or address, its value directly increases, proving in-place modifications are possible when using pointers or references.  

### Algorithm  
1. Start  
2. Define function `swap(int *x, int *y)`  
3. Use temporary variable to exchange `*x` and `*y`  
4. Call function with addresses of variables from `main()` (`swap(&a, &b)`)  
5. Print updated values in `main()`  
6. Also define increment function taking pointer/reference and add to variable  
7. Stop  

***

## **Conclusion**  
Through these programs, the basics of C++ pointers are clearly explained:  

- **Program 1** demonstrates accessing addresses and dereferencing.  
- **Program 2** shows how pointers can **alter variable contents** and access arrays.  
- **Program 3** utilizes **pointer arithmetic** for traversing arrays.  
- **Program 4** clarifies that call by value **does not change originals**.  
- **Program 5** highlights how using pointers/references allows **real-time modification** of variables from within functions.  

Together, these examples establish pointers as powerful tools in C++ for memory-level data management, function argument handling, and efficient array operations.  
[3](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/85057922/a2135a41-4c5e-4c81-a882-1c2f2246b32d/exp93.cpp)
[4](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/85057922/4b4ba00a-77c3-4cbe-800c-d43e8fb5e2bd/exp94.cpp)
[5](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/85057922/3ee9ef78-aaa5-48d5-9592-88ea183af91d/exp95.cpp)
