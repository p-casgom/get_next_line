# get_next_line

### Description:

Write a function that returns a line read from a file descriptor.

`char *get_next_line(int fd);`

### Requirements:
- Repeated calls (e.g., using a loop) to your get_next_line() function should let
you read the text file pointed to by the file descriptor, one line at a time.
- Your function should return the line that was read.
If there is nothing left to read or if an error occurs, it should return NULL.
- Make sure that your function works as expected both when reading a file and when
reading from the standard input.
- Please note that the returned line should include the terminating \n character,
except when the end of the file is reached and the file does not end with a \n
character.
- Add all the helper functions you need in the get_next_line_utils.c file.
- Allowed external functions: read, malloc, free.

### Learning process:

The [42 Get Next Line Guide (String Approach)](https://medium.com/@lannur-s/gnl-c3cff1ee552b) series of articles were extremely helpful for me to understand how to approach **get_next_line**, i.e., structuring the project, proper memory management, and creative thinking/problem-solving. I must give credit to the writer not just for her amazing article, but also for the approach she took, as I implemented it on my own project, and some of my functions are based on her own original code.

During this project I also came across the term ["memory-ownership"](https://stackoverflow.com/questions/60046802/understanding-memory-ownership-models-in-c). This concept has been helpful for me to understand and appreciate programmers' decisions for creating specific functions, and which of these take care of allocating and/or freeing memory. This was crucial for me to avoid memory leaks and double freeing.

### Testing:

gnlTester, fsoares. See [Francinette](https://github.com/WaRtr0/francinette-image).

*Didn't pass francinette --strict
