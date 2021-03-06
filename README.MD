# VisDaS
### **Vis**ualizing **Da**ta **S**tructure


A python package for visualizing data structures and its contents

[Data structures](https://en.wikipedia.org/wiki/Data_structure) form an essential part of computer science. A data structure helps in organizing, managing and storing data in a computer for efficient access and modification. 

Visualization of data structure makes it easy to understand the data structure and how elements of that data structure are connected to each other. 

This package helps in providing an easy way to get an image of visualization of the data structure and its elements. You can also perform basic operations on your array to understand the result of the function  

It provides a way to visualize the contents of data structure and how the elements of data structure are related to each other. 

The package currently supports visualization of following data structures : 
+ **[Array](https://en.wikipedia.org/wiki/Array_data_structure)**


## Examples of How To Use

```Python
from visdas import Array

arr = Array([10,15,20,25])
arr.insert(30)
arr.generate("array.png")
```

### array.png

![array](tests/array.png)

## Function Description

#### Array 
+ get()

    Returns the array 
    ```Python
    arr = Array([100,200,300])
    print(arr.get())
    ```
    
+ insert(element,index) 

    Inserts an element at given index. If the index is not specified then it appends the element to end of array.
    ```Python
    arr = Array()
    arr.insert(30)
    # Appends 30 to end of array
    print(arr.get())
    # [30]
    arr.insert(0,10)
    # Inserts 10 at the index 0 of array
    print(arr.get())
    # [10,30]
    ```
    
+ remove(element) 

    Removes the first occurence of an element from the array
    ```Python
    arr = Array([10,20,30,40])
    arr.remove(30)
    # Removes the first occurence of 30 
    print(arr.get())
    # [10,20,40]
    ```
+ len()

    Returns the length of array
    ```Python
    arr = Array([12,14,16])
    print(arr.len())
    # 3
    ```
    
+ generate()

    Generates the image of array with specifies parameters
    ```Python
    arr = Array([12,14,16])
    arr.generate("myArray.png","black","white")
    ```
    ![myarray](tests/myArray.png)
