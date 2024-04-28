---
type: note
---
02/13/2023 14:44

Tags: #Embeded_Systems 

[[Assembly]] directives are not instructions, but they do provide information to the assembler. They are used to designate the start and end of the file and procedures as well as designate memory blocks and symbols. 

Directive | Function
----|----
*AREA* | Make new code/data block
**ENTRY** | Start program execution
ALIGN | Designate memory block for code/data
DCB | Allocate $\ge1$ bytes of data
DCW | "" halfwords
DCD | "" words
SPACE| Allocate zeroed block of arbitrary size
FILL| Allocate block and fill with given value
EQU| Give symbol name to constant
RN| Give symbol name to register
EXPORT| Declare symbol, make visible outside source file
IMPORT| Import symbol from another file
INCLUDE/GET| Include separate source file in current file
PROC| Start a function
ENDP| End a function
**END**| End the file

**Bold**: Required for all source files
*Italics*: 

### AREA
The `AREA` directive designates the start of a code or data section and is processed by the [[Linker]]. These are indivisible units, and each file must have at least one code section. It defines the name, type, and readablity of the section. Each name must be unique in within the file. 

>[!note]
>By default, a code area can only be `READONLY`, and a data area must be `READWRITE`

---

### PROC and ENDP
These two directives mark the start and end of a [[Function]]. One source file can contain many functions, but they cannot be nested. 

---