    === ASM-BASIC DOCUMENTATION ===

ASM-BASIC is an Assembly dialect that's mostly fine for most of the basic
computers. This is ASM-BASIC's documentation:

    === DATA STRUCTURE ===

In ASM-BASIC, data is made from 256  cells that can store 16-bit data.
There's a pointer that starts at cell #1, and there's 3 additional data
storage: a stack that can store 32-bit data (and 64 values), and a
queue that can store 32-bit data, too (and 64 values). Also, all the
commands need to run between these commands:
===
start
halt
===
When ran, this will give this error:
"CODE IS INSUFFICIENTLY POLITE"
Because, the program needs to politely ask the code, so this is valid:
===
please start
halt
===
The "please" keyword's needed to be put in front of another at least
1 time and at most 10 times. If more than 10, the program will output
"CODE IS OVERLY POLITE"
Here's an introduction:

    === COMMENTS ===

To comment the code, here are all the ways shown in a code:
===
please start
// 1-line comment v1
# 1-line comment v2
rem Retro 1-line comment
/*
Multi-line comment!
*/
\* Another way to do it *\
/* And the final way *\
halt
===

    === MOVING THE POINTER ===

The pointer can be moved by these 2 commands:
"mov fwd 1" = Moves the pointer right by 1.
"mov bck 1" = Moves the pointer left by 1.
"mov to 2" = Moves pointer to cell #2.
Note: The "n" in "mov fwd/bck n" is first gone through "n mod 256" operation,
then used.

    === STORING DATA ===

To store data to a cell, the pointer needs to be on the cell. Here's
some ways to do it:
"inc 1" = Increments the cell at the pointer by 1.
"dec 1" = Decrements the cell at the pointer by 1.
"sqr 2" = Multiplies the cell at the pointer by itself 2 times.
"cb 2" = Multiplies the cell at the pointer by itself 3 times 2 times.
"reset" = Sets the cell at the pointer to 0.
"set 1" = Sets the cell at the pointer to 1.
"cell" = Cell at the pointer as a variable/data type
Note: If any cell's binary value is higher than 256 or lower than 0,
it's replaced with its absolute value and gone through "n mod 256" operation.
Also, "code" command is the whole code as a data type/variable.

    === LOOPS ===

Loops can be used with this logic:
"start loop" = Jumps past the matching "end loop" if the cell at the pointer is 0.
"end loop" = Jumps back to the matching "start loop" if the cell at the pointer isn't 0.

    === STACK MANAGEMENT ===

To push/pop or get data from a stack, use these:
"push stack" = Appends the cell at the pointer to the top of stack.
"pop stack" = Deletes the stack's top value, basically pop it.
"swap stack" = Swaps the locations of the top value of the stack and the element under it.
"sortas stack" = Sorts the stack according to the integers stored ASCENDING.
"sortde stack" = Sorts the stack according to the integers stored DESCENDING.
"shuffle stack" = Shuffles the stack, just like the "random.shuffle(list)" method in Python 3.
"set stack" = Sets the cell at the pointer the top value of the stack.

    === QUEUE MANAGEMENT ===

The queue is almost the same as the stack, so memorizing the commands
is much simpler.
"push queue" = Appends the cell at the pointer to the top of queue.
"pop queue" = Deletes the queue's bottom value, basically pop it.
"swap queue" = Swaps the locations of the bottom value of the queue and the element on top of it.
"sortas queue" = Sorts the queue according to the integers stored ASCENDING.
"sortde queue" = Sorts the queue according to the integers stored DESCENDING.
"shuffle queue" = Shuffles the queue, just like the "random.shuffle(list)" method in Python 3.
"set queue" = Sets the cell at the pointer the bottom value of the queue.

    === INPUT AND OUTPUT ===

There is 4 valid commands to get input from the user and output data.
"scan int" = Gets an integer from the user and stores it at the cell at the pointer.
"scan ascii" = Gets a text from the user and stores its first letter's Unicode integer value at the cell at the pointer.
"print int" = Outputs the integer stored on the cell at the pointer without a newline.
"print ascii" = Outputs the integer's Unicode ASCII value stored on the cell at the pointer without a newline, basically "." on Brainf**k.

    === LOGIC GATE SIMULATION ===

With some commands, logic gates can be simulated. For this, True value
is 1, and the False value is 0.
"buffer" = Sets the cell at the pointer 0 if it's not 1.
"not" = Sets the cell at the pointer 0 if it's 1, else 1.
"and" = Sets the cell at the pointer 1 if the 2 cells on its left are 1, else 0.
"or" = Sets the cell at the pointer 1 if one of the 2 cells on its left are 1, else 0.
"nand" = Sets the cell at the pointer 0 if the 2 cells on its left are 1, else 1.
"nor" = Sets the cell at the pointer 0 if one of the 2 cells on its left are 1, else 1.
"xand" = Sets the cell at the pointer 1 if the 2 cells on its left are the same, else 0.
"xor" = Sets the cell at the pointer 1 if only one of the 2 cells on its left are 1, else 0.
"xand" = Sets the cell at the pointer 0 if the 2 cells on its left are the same, else 1.
"xor" = Sets the cell at the pointer 0 if only one of the 2 cells on its left are 1, else 1.

    === VARIABLES ===

You can define a variable with these methods:
"var x = 0" = Now, x is 0 and can be changed.
"let y = 0" = But y is a constant, it can't be changed.
"x = 1" = Now, x is changed!
"let x = 2" = Now, x is converted to a constant.
"var y = 0" = And y is converted to a normal variable.
"set x" = Now, the cell at the pointer is x, so 2.
Note: Variables can't have the names of keywords like "cell" or "let".
Also, arithmetic can be done with variables:
+ = Addition
- = Subtraction
* = Multiplication
/ = Division
% = Modulo
^ = Exponentation
: = Integer Division
Finally, logic gate simulation can be made (as 1 = True, 0 = False):
n == n = Equal to
n != n = Not equal to
n < n = Less than
n > n = Greater than
n && n = And logic gate
n || n = Or logic gate
n %& n = Xand logic gate
n %| n = Xor logic gate
n !& n = Nand logic gate
n !| n = Nor logic gate
n %!& n = Xnand logic gate
n %!| n = Xnor logic gate
? n = Buffer logic gate
! n = Not logic gate

    === FUNCTION DEFINITIONS ===

You can define a function with this setup:
===
please start
def as multiply n # a function's defined with the name of "multiply" and 1 variable/number input as "n".
var x = cell * n # define "x" as the cell at the pointer times function input
set x # set cell at the pointer as x, so multiply cell at the pointer by given "n" input
end def # end function definition
===
Now, let's try it:
===
set 5 # set cell as 5
multiply 5 # multiply cell by 5
print int # print cell
===
Output: "25"
Because 5 * 5 = 25 (5x5=25).

    === CONTROL FLOW ===

You can change the control flow by these commands:
"goto 1" = Goes to line 1 and continue execution there, basically "GOTO N" in AppleSoft BASIC.
"jmp 1" = Same as goto but different name to optionally decrease code readability.
"goto a if b is n" = Goes to line a if cell b is n.
"jmp a if b is n" = Same as "goto a if b is n" but the same intention with "jmp 1".
"inc c if b is d" = Increments cell at the pointer by c if cell b equals d.
"dec c if b is d" = Decrements cell at the pointer by c if cell b equals d.
"print int if b is e" = Outputs the integer stored on the cell at the pointer without a newline if cell b equals e.
"print ascii if b is e" = Outputs the integer's Unicode ASCII value stored on the cell at the pointer without a newline if cell b equals e.

    === SUPERIOR TO THESE ===

ASM-BASIC is superior to these progamming languages:
Brainf**k: Has nearly same data structure but with way more commands.
Hexagon says jump to line a if cell b is n and increment cell b by c if cell b equals d and output cell b if cell b equals e.: Can be interpreted in ASM-BASIC with the commands in the Control Flow part.
Deadfish: Has the same commands with it and has more
ΙΧΘΥΣ: Same reason as Deadfish
Ook! = Because it's the same as Brainf**k
NOP = It does nothing and ASM-BASIC does things.

    === EXAMPLE PROGRAMS ===

Cat (returns input as output):
please start
# This program is only valid for integers.
scan int
print int
halt

Looping Counter:
1 please start
2 print int
3 inc 1
4 goto 2
5 halt

Powers of 2:
1 please start
2 print int
3 sqr 2
4 goto 2
5 halt

Truth Machine (returns 0 if input's 0, returns 11111... if input's 1):
1 please start
2 scan int
3 let x = cell
4 mov fwd 1
5 goto 8 if x is 0
6 print int
7 halt
8 set 1
9 print int
10 goto 9
11 halt

Fibonacci Sequence:
1 please start
2 var x = 0
3 var y = 0
4 inc 1
5 print int
6 print int
7 var z = x + y
8 set z
9 print int
10 x = y
11 y = z
12 goto 7
13 halt

ASCII Art Drawing Space:
1 please start
2 input ascii
3 goto 2
4 halt

Turing Machine:
Theoretically, it can be simulated with only the NAND logic gate,
which can be simulated infinitely in ASM-BASIC, even if it's inefficient.
