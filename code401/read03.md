# FilelO & Exceptions

## Read & Write Files in Python

### What is a file?

- Three main parts
  - Header: metadata about the contents of the file (name, size, type and so on)
  - Data: contents of the file as written by the creator or editor
  - End of file(EOF): special character that indicates the end of the file


### File paths

- Folder path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)

- File name: the actual name of the file
- Extension: the end of the file path pre-pended with a period used to indicate the file type such as .txt or .md

#### Opening a file

```
file = open('file_im_opening.txt')
```

#### Closing a file

```
file.close()
```

### Line endings

- Line endings are used to specify a new line or the end of a line
- Carriage Return or \r and Line Feed \n are end of line characters according to the ASA

### Ensuring files are closed
- try and finally code block

**Always make sure that an open file is properly closed**

### Using with 
- only runs the code until the code below is no longer indented

### r w rb or wb
- r: open for reading (default)
- w: open for writing, truncating (overwriting) the file first
- rb or wb: open in binary mode

### Buffered Binary Files Types

> A buffered binary file type is used for reading and writing binary files. Here are some examples of how these files are opened:

```
open('abc.txt', 'rb')

open('abc.txt', 'wb')

```

------------------------------------------------

# Exceptions in Python

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception

In Python, syntax errors occur when the parser detects an incorrect statement and an arrow will indicate us where the parser ran into the syntax error

The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.