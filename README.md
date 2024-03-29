Description:
A MIPS program that reads a string of up to 1000 characters from user input.
The string consists of one or more substrings separated by comma. Spaces or tabs at the
beginning or end or around commas are ignored, those spaces or tabs should stay. For each
of the substring, if it is a hexadecimal string, i.e. it has only the characters from '0' to '9'
and from 'a' to 'f' and from 'A' to 'F', and it is of no more than 8 characters, the program
prints out the corresponding unsigned decimal integer. If the hexadecimal string has more
than 8 characters, the program prints out the string of “too large”. Otherwise, the program
prints out the string of “NaN”. Empty strings before the first comma, between commas or
after the last comma are also considered “NaN”. The output should be separated by
commas in the same way as the input.

The program must have the following 3 subprograms.

Subprogram 1:
It converts a single hexadecimal character to a decimal integer. Registers must be used
to pass parameters into the subprogram. Values must be returned via registers.

Subprogram 2:
It converts a single hexadecimal string to a decimal integer. It must call Subprogram 1
to get the decimal value of each of the characters in the string. Registers must be used
to pass parameters into the subprogram. Values must be returned via the stack.

Subprogram 3:
It displays an unsigned decimal integer. The stack must be used to pass parameters into
the subprogram. No values are returned.

The main program must call Subprogram 2 for conversion and call Subprogram 3 for
output.
