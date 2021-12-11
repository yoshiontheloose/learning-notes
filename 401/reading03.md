# FileIO & Exceptions

## Read & Write Files in Python

[Source](https://realpython.com/read-write-files-python/)

Files store data using bytes. The computer processes files by translating them into binary.

3 Main parts of a file:

- Header - file content metadata/info (file name, size, type)

- Data - Contents written by creator

- End of File - (EOF) End of the file indicated by a special character

**File Paths**

"The file path is a string that represents the location of a file."

3 Parts of a file path

- Folder Path

- File Name

- Extension

**Line Endings**

Carriage Return - CR or /r

Line Feed - LF or /n

**Character Encodings**

Encoding translates byte data to characters readable by humans.

Two most common encodings: ASCII and UNICODE

**Opening and closing a file in Python**

Function to open/work with a file: `open()`

***Always close an open file properly***

- When an application or script is terminated, the file will close eventually, but no telling when. Resource leaks and unwanted behavior can occur when a file is not closed properly.

Ways to close -

try-finally block:

```
reader = open('dog_breeds.txt')
try:
    # Further file processing goes here
finally:
    reader.close()
```

with statement

```
with open('dog_breeds.txt') as reader:

    # Further file processing goes here
```

Use with statement as defaut because it allows for cleaner code.

## Exceptions in Python

[Source](https://realpython.com/python-exceptions/)

---

# Videos

## Read & Write Files in Python - Companion Video

[Source](https://realpython.com/courses/reading-and-writing-files-python/)

# Bookmark/Skim

## Reading and Writing Files in Python Quiz

[Source](https://realpython.com/quizzes/read-write-files-python/)


[<<<Back](README.md)
