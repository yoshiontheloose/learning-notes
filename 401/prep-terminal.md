# The Command Line

## Tasks

Working as a tech professional will often involve interacting with the terminal on your computer.

This pre-work will introduce you to some of the more common commands involved in traversing directories and manipulating files on your computer.

## Submitting Your Work

For each of the following segments of [Bash Command Line Tutorials](https://ryanstutorials.net/linuxtutorial/) on ryanstutorials.net, completely read through and complete each of the activities in your own terminal. As you complete each segment’s activities, take a moment to document your learnings and observations.

---
---

## [The Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php) - What is it, how does it work and how do I get to one

The command line, better known to me as terminal, is a system interface navigated by text commands.

How to open terminal on a Mac:

- Applications -> Utilities -> Terminal

- _Command + Space_ to bring up Spotlight and search

*Shell* - "..part of the operating system that defines how the terminal will behave and looks after running (or executing) commands"

*Bash* - Bourne Again Shell. Very common.

*echo* - A command to display messages.

- *echo $SHELL* - find out current shell

---

## [Basic Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php) - An introduction to the Linux directory system and how to get around it

### Commands

***pwd*** - print working directory. Displays current directory

***ls*** - list. What is in the current directory.

- ***ls -l*** - files in the current directory with more info. (long listing)

- ***ls /etc*** - list of content in the directory

- ***ls -l /etc*** - long listing of directory

- ***cd*** - "change directory." Without arguments, goes to home directory

Path Builders/Arguments

- ***~*** - Shortcut to home directory

- ***. (just a dot)*** - Refers to current directory. Ex: ./Documents

- ***.. (double dot)*** - Refers to parent directory. "The go backwards button"

### Paths

**Path** - The way to a file or directory

**Root Directory** - Top of the hierarchy. Noted with one forward slash /

**Absolute Path** - location relative to the root directory. Begin with forward slash /

**Relative Path** - location relative to where you currently are. No slash.

---

## [More About Files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php) - Find out some interesting characteristics of files and directories in a Linux environment

Everything is a file!

Linux is case sensitive. Files can have the same name with different case letters.

Spaces in file names are tricky because the command line uses spaces to separate arguments.

- Can use quotes or escape characters for the file that has spaces

Hidden files can be created by beginning the name with a single dot(.)

- Rename/remove the dot to unhide.

- ls command will not list hidden files. Use ls -a to show hidden files.

File extensions:

- .exe -executable file or program

- .txt - text file

- .png, .gif, .jpg -image files

### Commands

***file*** - find info on the file type

***ls -a*** - directory contents with hidden files

---

## [Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php) - Learn how to make the most of the Linux commands you are learning

**Manual Pages** - "pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept."

### Commands

***man \<command to look up>*** - brings up manual pages

- press Q to quit

***man -k \<search term>*** - keyword search

***/\<term>*** - keyword search on a particular page

***n*** - goes to next found search term after searching

---

## [File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php) - How to make, remove, rename, copy and move files and directories

Be organized with structures.

### Commands

***mkdir*** - "make directory"

- ***-p***

- ***-v*** - tells us what it is doing

***rmdir*** - "remove directory"

- can also use -p -v

***touch*** - makes a blank file

***cp*** - copies a file

- ***cp \<source> \<destination>***

***mv*** - moves a file

- ***mv \<source> \<destination>***

  - use same directory as source for destination with a different name to rename file at same time

***rm*** - "remove." deletes a file.

- ***rm -r*** - "recursive" remove a directory and all files in it

-***rm -ri*** - "interactive" prompts before removing each file with option to cancel the command

**"whenever we refer to a file or directory on the command line it is in fact a path"**

---

## [Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php) - A quick reference for the main points covered in this tutorial

***jobs*** - current processes in the background

[<<<Back](README.md)