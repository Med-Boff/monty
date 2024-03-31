***Monty Program README***

--Overview--

The Monty program is a bytecode interpreter for the Monty programming language. It allows users to execute Monty bytecode files containing instructions to be interpreted and executed.

--Usage--
To run the Monty program, use the following command:

monty file
Where file is the path to the file containing Monty bytecode.

--Error Handling--

If the user does not provide a file or provides more than one argument to the program, the program will print an error message.


--USAGE-- 
monty file

If it's not possible to open the file specified by the user, the program will print the error message:

Error: Can't open file
followed by a new line, and exit with the status EXITFAILURE, where <file> is the name of the file.

--Execution--
The Monty program runs the bytecodes line by line and stops if either:

It executes every line of the file properly.
It finds an error in the file.
An error occurs during execution.

--Memory Management--
If the program can't allocate more memory using malloc, it will print the error message:

Error: malloc failed
followed by a new line, and exit with status EXITFAILURE.

The program strictly uses malloc and free for memory allocation and deallocation, and it's not allowed to use any other function from the malloc family (realloc, calloc, etc.).

--Notes--
Line numbers always start at 1 in Monty bytecode files.

--Author--
This Monty program was created by Med-Boff
