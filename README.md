Function that returns a line read from a file descriptor.

Project developed in C language.

The project follows the 'norma' (Norminette).

Calling this get_next_line function repeatedly will allow you to read the contents of the file pointed to by the file descriptor, line by line, to the end.

This function will return the line that was just read. If there is nothing more to read or if an error has occurred, it will return NULL.

The returned line will end with the character \n (line break), except if the end of the file has been reached and it does not end with a character \n(line break).

##The function prototype is:

`char *get_next_line(int fd);`

##Requirements:

The program compiles with the -D BUFFER_SIZE=xx flag. This flag is used to determine the buffer size of the reads of the get_next_line() function.

The program compiles with and without the flag (-D BUFFER_SIZE=xxx). By default its value will be 42.

##Functions allowed:

- read
- malloc
- free

##Specifics restrictions:

- Libft is not allowed
- lseek is forbidden
- Global variables are not allowed

##Bonus part: 

The project has to be implemented with a single static variable and it should be able to manage multiple fd at the same time.