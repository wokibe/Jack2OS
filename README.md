## Bootstrap for JackOS

The book proposes to implement the required OS classes in isolation in any
desired order, together with the precompiled \*.vm files.

I think, it is a didactic better strategy to implement the classes in 10 steps
in such an order, that they depend only on already developed classes, and not
using the precompiled \*.vm files. Of course, the _**Sys**_ class has to be
adapted in each step.

1. _**Memory**_
2. _**Array**_
3. _**Math**_
4. _**String**_
5. _**Output**_
6. _**Screen**_
7. _**Keyboard**_
8. _**Sys**_
9. Memory leak tests
10. Tests to force all OS errors

I added a class _**Util**_, that contains some functions, which I found missing
or which can be shared by the other classes
