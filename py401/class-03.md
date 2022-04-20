# [Reading-Notes](https://alsosteve.github.io/reading-notes/)
Code Fellows Python 401

# Read: 03 - FileIO & Exceptions

## [Read & Write Files in Python](https://realpython.com/read-write-files-python/)
> A **_file_** is a contiguous set of bytes used to store data.
### Components of a file:
  - **Header**: metadata about the contents of the file (file name, size, type, and so on)
  - **Data**: contents of the file as written by the creator or editor
  - **End of file (EOF)**: special character that indicates the end of the file

### File Paths
  - **_Folder Path_**: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
  - **_File Name_**: the actual name of the file
  - **_Extension_**: the end of the file path pre-pended with a period (.) used to indicate the file type

### Working on files
#### Steps:
``` python
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```
1. Open: to work on a file you need to open it
2. Manipulate file
3. Close: It’s important to remember that it’s your responsibility to close the file

#### With Statement
``` python
with open('dog_breeds.txt') as reader:
    # Further file processing goes here
```
The with statement automatically closes the file once it leaves the with block, even in cases of error.

#### types of opens
| CHARACTER | MEANING |
| --- | --- |
| 'r' | Open for reading (default) |
| 'w'	 | Open for writing, truncating (overwriting) the file first |
| 'rb' or 'wb' | Open in binary mode (read/write using byte data) |

#### Reading and Writing Opened Files

| Method | What It Does |
| --- | --- |
|.read(size=-1) |	This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read. |
| .readline(size=-1) |	This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read. |
| .readlines() |	This reads the remaining lines from the file object and returns them as a list. |

## [Exceptions in Python](https://realpython.com/python-exceptions/)
> An **_exception error_** is a type of error occurs whenever syntactically correct Python code results in an error.
- It works like a catch in JavaScript

* raise allows you to throw an exception at any time.
* assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
* In the try clause, all statements are executed until an exception is encountered.
* except is used to catch and handle the exception(s) that are encountered in the try clause.
* else lets you code sections that should run only when no exceptions are encountered in the try clause.
* finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

``` python
try:
    linux_interaction()
except AssertionError as error:
    print(error)
else:
    try:
        with open('file.log') as file:
            read_data = file.read()
    except FileNotFoundError as fnf_error:
        print(fnf_error)
finally:
    print('Cleaning up, irrespective of any exceptions.')
```

## [Video:Read & Write Files in Python - Companion Video](https://realpython.com/courses/reading-and-writing-files-python/)

## Bookmark and Review
- [Reading and Writing Files in Python Quiz](https://realpython.com/quizzes/read-write-files-python/)
