# FileIO & Exceptions

## Read & Write Files in Python

[Source](https://realpython.com/read-write-files-python/)

Files store data using bytes. The computer processes files by translating them into binary.

3 Main parts of a file:

- Header - file content metadata/info (file name, size, type)

- Data - Contents written by creator

- End of File - (EOF) End of the file indicated by a special character

**File Paths**:

"The file path is a string that represents the location of a file."

3 Parts of a file path

- Folder Path

- File Name

- Extension

**Line Endings**:

Carriage Return - CR or /r

Line Feed - LF or /n

**Character Encodings**:

Encoding translates byte data to characters readable by humans.

Two most common encodings: ASCII and UNICODE

### **Opening and closing a file in Python**

Function to open/work with a file: `open()`

***Always close an open file properly***

- When an application or script is terminated, the file will close eventually, but no telling when. Resource leaks and unwanted behavior can occur when a file is not closed properly.

**Ways to close**:

*try-finally block:* -

```markdown
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

*with statement* -

```markdown
with open('dog_breeds.txt') as reader:

    # Further file processing goes here
```

Use *with statement* as defaut because it allows for cleaner code and closes the file when it leaves the with block.

*mode* - Second argument for with/open statement. String form. States how to open the file.

|Most common used modes |  |
| --- | ---  |
| 'r' | Open to read |
| 'w' | Open to write, overwrites the file |
| 'rb' or 'wb' | Open in binary (read or write) |
| 'a' | append to a file

With Statement + mode EX:

``` markdown
with open('dog_breeds.txt', 'r') as reader:
    # Further file processing goes here
```

**Three Categories of File Objects** -

Text files

- open() returns a TextIOWrapper file object

Buffered binary files

- open() returns a BufferedReader or BufferedWriter file object

Raw binary files

- open() returns a FileIO file object

### Reading Opened Files

Method | Description
--- | ---
`.read(size=-1)` | Reads entire file. Based on # of size bytes
`.readline(size=-1)` | returns a line from the file when called
`.readlines()` | returns all the lines from file as a list with each element as a line in the file

Additional source: [edureka]

`end=''` - prevents Python from adding to the printed text and only prints what is read from the file.

EX:

```markdown
with open('dog_breeds.txt', 'r') as reader:
for line in reader:
print(line, end='')
```

### Writing files

| Method | What It Does |
--- | ---
| `.write()` | writes string to the file |
| `.writelines(seq)` | Writes sequence to the file |

`__file__` - "returns the path relative to where the initial Python script was called"

### Create context manager

`__enter__()` - invoked when calling *with* statement

`__exit__()` - called when exiting from the *with* block

---

## Exceptions in Python

[Source](https://realpython.com/python-exceptions/)

---

# Videos

## Read & Write Files in Python - Companion Video

[Source](https://realpython.com/courses/reading-and-writing-files-python/)

# Bookmark/Skim

## Reading and Writing Files in Python Quiz

[Source](https://realpython.com/quizzes/read-write-files-python/)

## Searched Source(s)

[edureka](https://www.edureka.co/blog/python-readline/)

[<<<Back](README.md)
