*This project has been created as part of the 42 curriculum by <pdiniz-l>.*

# get_next_line

## Description

**get_next_line** is a C library that provides a function to read a file descriptor **line by line**, returning one line per function call.

The goal of this project is to implement a robust, memory-safe solution that handles buffered reading, preserves state between calls, and correctly manages edge cases such as end-of-file, missing newline characters, invalid file descriptors, and allocation failures.

This implementation follows the specifications of **Get Next Line v13** from the 42 curriculum and is written in compliance with the project constraints and allowed functions.

---

## Instructions

### Compilation

The project must be compiled while defining the `BUFFER_SIZE` macro, which controls how many bytes are read per call to `read`.

Example:

```bash
cc -Wall -Wextra -Werror -D BUFFER_SIZE=32 get_next_line.c get_next_line_utils.c
```
You may change the value of `BUFFER_SIZE` to test different buffer behaviors.
