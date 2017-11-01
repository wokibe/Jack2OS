### Step01 : _**Memory**_

* **Memory.jack**
  * function void **init**(): for internal use only
  * function int **peek**(int address): returns the value of the main memory at
  this address
  * function void **poke**(int address, int value): sets the contents of the
  main memory at this address to value
  * function Array **alloc**(int size): finds and allocates from the heap a
  memory block of the specified size and returns a reference to its base address
  * function void deAlloc(Array o): De-allocates the given object and frees its
  memory space

  Added a function to allow a memory leak test:
  * function int **getFreeListAddr**(): returns the pointer to the first free
  block

* **Util.jack**

  added:
  * function int **getFreeListSize**(): returns the sum of all free heap block

* **Sys.jack**
  * function void **init**(): calls the init functions of _**Memory**_ and
  _**Util**_ and then calls the **Main.main**() function. For internal use only
  * function void **halt()**: halts the program execution
  * function void **error**(int errorCode): ignores the error code (as we can't
  output yet) and halts

* **Main.jack**
  * change to use **peek**'s and **poke**'s instead of the corresponding Array
  methods
  * Added some code to check if there is a memory leak after some
  **Memory.alloc**'s and **Memory.deAlloc**'s'

* **Memory.tst**
  * Added check of the result of the memory leak test

* **Memory.cmp**
  * Added the expected memory leak test result
