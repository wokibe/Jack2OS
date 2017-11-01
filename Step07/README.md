### Step06 : _**Keyboard**_

* **Keyboard.jack**
  * function void **init**(): for internal use only
  * function char **keyPressed**(): returns the character of the currently
  pressed key on the keyboard; if no key is currently pressed, returns 0
  * function char **readChar**(): waits until a key is pressed on the keyboard
  and released, then echoes the key to the screen and returns the character
  of the pressed key
  * function String **readLine**(String message): prints the message on the
  screen, reads the line (text until a newline character is detected) from
  the keyboard, echoes the line to the screen, and returns its value. This
  function also handles user backspaces
  * function int **readInt**(String message): prints the message on the screen,
  reads the line (text until a newline character is detected) from the
  keyboard, echoes the line to the screen, and returns its integer value
  (until the first non-digit character in the line is detected). This
  function also handles user backspaces

* **Sys.jack**
  * enable **Keyboard.init**()

* **Util.jack**
  Added:
  * function boolean **isPrintable**(char c): returns true if '!' <= c <= '~'
