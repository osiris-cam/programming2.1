# Classification of Arrays
-------------------------------------------------------------------------------------------------------------------------
## [What is an array?](https://www.geeksforgeeks.org/introduction-to-arrays/)  

When we talk about an array we are referring to an ordered and finite set of elements, they are also known as matrices (in mathematics) and tables (in financial calculations). They have the property of being ordered, that is, the first element, the second, the third, etc. can be identified. It is important to note that the elements that an array has are homogeneous (of the same data type), that is, that its elements can be of type string, integer type, floating.

![image0](https://miro.medium.com/max/3184/1*X0Dg7QfSYtWhSAu-afi8-g.png)

## [One-dimensional array](https://www.geeksforgeeks.org/introduction-to-arrays/)

The simplest array is the one-dimensional array or also called vectors. They are called one-dimensional because it only requires an index to access the component.
Arrays consist of essential characteristics, for example they have a subscript (1,2,3, n) that indicates their position in the array order. Furthermore, the elements of this vector are referenced by their subscripts (their relative position of the value).In addition, the arrays are stored in the PC's central memory in a certain order, so an array of 6 numbers is represented graphically by 6 successive memory locations.

To better understand this concept, we show the following image:

![imagen1](https://media.geeksforgeeks.org/wp-content/uploads/array-2.png)

The syntax of an array in C is as follows:

**ArrayElementType ArrayName [numberElements];**
Example: **int vectorEnteros [6];**

In the previous example we observe that an array of integer type has been created that will contain 6. Although the number in the declaration is 6, the element vectorInt [6] will not exist because in C our indices are given by 0,1,2,3,4,5. 
Example of program in C:
```
#include <stdio.h>
#include <stdlib.h>
// Example will learnprogramming.com
int main () {
int carNumber [24];
int R;
R = 2;
carNumber [R] = 57;
printf ("Time R is% d \ n", R);
printf ("The number of cars in hour% d was% d cars \ n", R, number of Cars [R]);
return 0;
}


```

## [Multidimensional array](https://www.geeksforgeeks.org/introduction-to-arrays/)

Because the memory of the pc is linear, a multidimensional array must be aligned for its arrangement in the storage. With these arrays it is possible to create them with more than one dimension, that is, it can be made up of m x n elements, such as three-dimensional, four-dimensional structures, etc.

![imagen3](https://i.stack.imgur.com/whdnE.jpg)

Siintaxis in C:
**VariableType ArrayName [dimension1] .[dimension2] [...] [dimensionN]**
Example: int A [3] [2]

Example of program in c:
```
#include <stdio.h>
#include <stdlib.h>

int main() {
int peoplebyhouse[5][25];
peoplebyhouse[3][24] = 4;
printf("The number of people per haouse 24 of the floor 3 is %d\n", peoplebyhouse3][24]);
return 0; 
}
```

Example in python:
```
for i in range(0,rows): ##This piece of code gonna add to list new  row
		m1.append([]) ##ading a new row according to respective number of rows
		m2.append([]) ##...
		r.append([])  ##The same to matrxi result
		for j in range(0,cols):
			m1[i].append(0) ##Adding a initial value to  matrix
			m2[i].append(0)
			r[i].append(0)
	print(('Matrix %ix%i\n')%(rows,cols)) ##Show some info
	print(m1)
	print(m2)

```
### Access to multidimensional matrix elements.
To access some element of the multidimensional array, we only make use of its subscripts (depending on their dimension). If it is two-dimensional, we will use counters i and j, if they are three-dimensional we add counter k. Also to have access we will make the use of for loops depending on the dimension of the array.

Example in c (nultiplication of matrix):

```
for (i=0; i<row_a; i++){ //we need to loop through each column of matrix 1 and multiply it by the rows of matrix 2. We need accumulators (j, k, i)
        for(j=0; j<colum_b; j++){
            result[i][j]=0;
            for(k=0; k<MAX; k++)
            {
                result[i][j]=(result[i][j]+(matrix1[i][k]*matrix2[k][j])); //operation, here te result is saving in the variable result 
            }
        }
	}
	printf ("MULTIPLICATION:\n:"); //print each element with iterators i and j
        for (i=0; i<row_a; i++){
        	printf("\n\f\f");// to give format
        	for(j=0; j<colum_b; j++){
            	printf("\t [%d]", result[i][j]);
        }
    }

```
Example in Python:
```
for i in range(0,rows): ##The program do some math to get the resultant matrix
		for j in range(0,cols):
			for k in range(0,cols):
				r[i][j] += m1[i][k]*m2[k][j]
	print(r) ##Print result and finish the program!
```

# Organization and Management of files

## Data flow
[Data flow](https://www.geeksforgeeks.org/what-is-dfddata-flow-diagram/) The flow of data of a system or a process is represented by DFD.
 It also gives insight into the inputs and outputs of each entity and the process itself. DFD does 
 not have control flow and no loops or decision rules are present.
 This diata flow has 4 components:
 * Process: Input to output transformation in a system takes place because of process function.
 * Data flow: describes the information transferring between different parts of the systems.
 * Warehouse: The data is stored in the warehouse for later use.
 * Terminator: is an external entity that stands outside of the system and communicates with the system.

## Files
[Files](https://techterms.com/definition/file)A file is a collection of data stored in one unit, identified by a filename.
 It can be a document, picture, audio or video stream, data library, application, or other collection of data.
 There are a lot of types of files, but in this file we are going to focused only in the text and the binary files.
 * [Text files](https://www.computerhope.com/jargon/t/textfile.htm): A text file is a computer file that only contains text and
  has no special formatting such as bold text, italic text, images, etc.
  ![Text files](https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/full_width/public/thumbnails/image/DR_SampleCSV_0.PNG)
 
 * [Binary files](https://whatis.techtarget.com/definition/binary-file): A binary file is a file whose content must be interpreted by a program
  or a hardware processor that understands in advance exactly how it is formatted. That is, the file is not in any externally identifiable
  format so that any program that wanted to could look for certain data at a certain place within the file. A progam (or hardware processor)
  has to know exactly how the data inside the file is laid out to make use of the file.
  ![Binary files](https://upload.wikimedia.org/wikipedia/commons/thumb/7/76/Wikipedia_favicon_hexdump.svg/1200px-Wikipedia_favicon_hexdump.svg.png)

## File managements
[File management](http://w.sunybroome.edu/basic-computer-skills/functions/file_management/2definitions.html) Is the process
 and act of creating an organized structure in which you store information for easy retrieval. In this text we are going to be focused on
 the file management of the C programs and the Python Programs.
 * [C](https://www.geeksforgeeks.org/basics-file-handling-c/):
   * Creation of a new file (fopen with attributes as “a” or “a+” or “w” or “w++”)
   * Opening an existing file (fopen)
   * Reading from file (fscanf or fgets)
   * Writing to a file (fprintf or fputs)
   * Moving to a specific location in a file (fseek, rewind)
   * Closing a file (fclose)

 * [Python](https://www.geeksforgeeks.org/file-handling-python/):
   * Opening of an existing file(open ()), but we use the next commands to indicat what we are going to do with this file.
     * “ r “, for reading.
     * “ w “, for writing.
     * “ a “, for appending.
     * “ r+ “, for both reading and writing
     For example:
```
     # a file named "pizza", will be opened with the reading mode. 
     file = open('pizza.txt', 'r') 
     # This will print every line one by one in the file 
     for each in file: 
	 print (each) 
```
   * Reading from a file (file. read())
   For example
```
# Python code to illustrate read() mode 
file = open("file.text", "r") 
print file.read() 
```
   * Creating a file 
```
# Python code to create a file 
file = open('pizza.txt','w') 
file.write("This is the write command") 
file.write("It allows us to write in a particular file") 
file.close() 
```
   * Closing a file (file.close())
   * Writing a file

```
# Python code to illustrate with() alongwith write() 
with open("file.txt", "w") as f: 
	f.write("Hello World!!!") 
```
   * Split a file
```
# Python code to illustrate split() function 
with open("file.text", "r") as file: 
	data = file.readlines() 
	for line in data: 
		word = line.split() 
		print word 
```

## ***Equipo***:
1. Osiris Cámara Salinas.
2. Victor Uribe Hernandez.. 
