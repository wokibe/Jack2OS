### Step06 : _**Screen**_

* **Screen.jack**
  * function void **init**(): for internal use only
  * function void **clearScreen**(): erases the entire screen
  * function void **setColor**(boolean b): sets a color
  (white = false, black = true) to be used for all further drawXXX commands
  * function void **drawPixel**(int x, int y): draws the (x,y) pixel
  * function void **drawLine**(int x1, int y1, int x2, int y2)
  draws a line from pixel (x1,y1) to pixel (x2,y2)
  * function void **drawRectangle**(int x1, int y1, int x2, int y2)
  draws a filled rectangle whose top left corner is (x1,y1) and
  whose bottom right corner is (x2,y2)
  * function void **drawCircle**(int x, int y, int r): draws a filled circle
  of radius r <= 181 around (x,y)

* **Sys.jack**
  * enable **Screen.init**()
