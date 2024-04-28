---
type: note
tags: [Embeded_Systems]
---
03/24/2023 14:41

  

When using a keypad as a [[General Purpose Input Output|GPIO]] input, the board will read the button presses by using three input pins connected to the columns and four output pins connected to the rows. A reference voltage is also connected to the columns. When a button is pressed, the [[CPU]] reads an input in the button's row. The button also connects the row conductor to the column. Since the rows are output pins, the CPU sets each row to zero successively. The row that is still logical one due to the button press is the row of the button press. Now the CPU knows the row and column of the button press, and therefore which button was pressed