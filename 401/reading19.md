# Automation

## Python Regular Expressions Tutorial

[Source](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)

**regex** - Regular Expressions. An arrangement of characters that checks a given string/text for a pattern. They help manipulate textual data.

To use them in your Python script, import the re module:

> `import re`

`match()` - returns a match object if the text matches the pattern. Only checks for a match at the beginning of the string.

`search()` - scans the given string/sequence for a match anywhere in the string

`group()` - returns string matched by the re. Allows you too pick parts of the matching text. Brackets `< >` will also allow you to create named groups.

"Greedy Matching" - A special character matching a lot of the search sequence when you don't want it to. `*?` will allow you to match as little text as possible.

"Non-greedy Matching" - Add a `?` after a qualifier to match minimally so as few characters as possible will be matched.

**Compilation Flags**:

`IGNORECASE` - Allows case insensitive matches

`DOTALL` - Allows `.` to match any character along with newline

`MULTILINE` - Allows start of string `^` and end of string `$` to match newlines

`VERBOSE` - Allows whitespace and comments within a regex for readability

## shutil

High level file operations like copying and archiving.

`copyfile()` - copies source contents to the destination. Will raise an IOError if it doesn't have permission to write to destination file.

`copymode()` - copy permissions from one file to another

`copytree()` - Used to copy a directory from one place to another. Copies files to the destination as it recurses through source directory tree. Destination directory cannot exist in advance.

[Source](https://pymotw.com/3/shutil/)

---

# Videos

## Automation Ideas

[Source](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)

## Automating Your Browser and Desktop Apps

[Source](https://www.youtube.com/watch?v=dZLyfbSQPXI)

---

# Bookmark/Skim

## Watchdog

[Source](https://pythonhosted.org/watchdog/)


[<<<Back](README.md)