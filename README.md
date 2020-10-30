# get_next_line

Function name get_next_line
Prototype int get_next_line(int fd, char **line);

Parameters
#1. file descriptor for reading
#2. The value of what has been read
Return value 
1 : A line has been read
0 : EOF has been reached
-1 : An error happened

External functs. read, malloc, free

Description Write a function which returns a line read from a file descriptor, without the newline.
• Calling your function get_next_line in a loop will then allow you to read the text available on a file descriptor one line at a time until the EOF.
• Make sure that your function behaves well when it reads from a file and when it reads from the standard input.
• Your program must compile with the flag -D BUFFER_SIZE=xx. which will be used as the buffer size for the read calls in your get_next_line. This value will be
modified by your evaluators and by moulinette.
• Compilation will be done this way : gcc -Wall -Wextra -Werror -D BUFFER_SIZE=32 get_next_line.c get_next_line_utils.c
• Your read must use the BUFFER_SIZE defined during compilation to read from a file or from stdin.
• lseek is not an allowed function. File reading must be done only once.
