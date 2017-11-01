### Step09 : Memory leak tests

* **Main.jack**

  Utility program the helps to investigate the behavior of **Memory.alloc**()
  and **Memory.deAlloc**() in action.

    * In test mode it generates 5 small arrays, fills them with an individual
    pattern and disposes them in a different order. it is possible
    to check the free list blocks after each dispose.

    * Additional the whole or partial heap structure may be printed.

    * In stress mode it perform several thousands of **alloc**'s and **deAlloc**'s
    of different sizes to prove, that no memory leaks exists.

* **Util.jack**

  * added:

  * function void **printFreeList**(): dumps the free list blocks (size and next)
  * function void **printHeapList**(int above): dumps address and size of heap
  blocks above some limit
