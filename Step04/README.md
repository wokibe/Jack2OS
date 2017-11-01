### Step04 : _**String**_

* **String.jack**
  * constructor String **new**(int maxLength): constructs a new empty string
  (of length zero) that can contain at most maxLength characters

  * method void **dispose**(): disposes this string

  * method int **length**(): returns the length of this string

  * method char **charAt**(int j): returns the character at location j of this
  string

  * method void **setCharAt**(int j, char c): sets the j-th element of this
  string to c

  * method String **appendChar**(char c): appends c to this string and returns
  this string

  * method void **eraseLastChar**(): erases the last character from this string

  * method int **intValue**(): returns the integer value of this string (or the
    string prefix until a non-digit character is detected)

  * method void **setInt**(int j): sets this string to hold a representation
  of j

  * function char **backSpace**(): returns the backspace character

  * function char **doubleQuote**(): returns the double quote (“) character

  * function char **newLine**(): returns the newline character

* **Util.jack**

  * Added:

  * function boolean **isNumeric**(char c): returns true, if ("0" <= c "9")

  * function boolean **isAlpha**(char c): tests if ("A" <= c <= "Z") |
  ("a" <= c <= "z")

* **Main.jack**

  * this test program needs the class _**Output**_ to display the results
  So this class has to be implemented for this step too

* **Sys.jack**

  * enable **Output.init**()

  * enable the errorCode output in **Sys.error**(errorCode)
