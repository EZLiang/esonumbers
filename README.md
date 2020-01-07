# esonumbers
An advanced esoteric language

_esonumbers is a very simple esoteric language._

An esonumbers program has 4 variables: I/O (stack), memory (number), position, and program (tape).

The program begins with position at the beginning and 0 in memory.

In execution:
 1. When the character at the current position is an `@`, end program and output I/O stack.
 2. When the chracter at the current position is equal to the value in memory, pop the item at the top of I/O and write it at the current position.
 3. When the chracter at the current position is _k_ more than the value in memory, set memory to the current value and jump right k. For each jumped over non-`@` character push its value onto the I/O stack and increment by 1.
 4. When the chracter at the current position is _k_ less than the value in memory, set memory to the current value and jump left k. For each jumped over non-`@` character push its value onto the I/O stack and decrement by 1.
