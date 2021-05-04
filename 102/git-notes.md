## Git is a DVCS. 
  * Relies on local operations/local disk
  * Every change in file or directory is tracked by Git
  * Makes it very hard for a snaphot of a committed file to be lost
  * includes GUI tools

_Git States_
  * Committed - Securely stored in a local database
  * Modified - Changed but not yet committed to database
  * Staged - Changed version to be committed in next snapshot

GUI - Graphical User Interface



##Version control system (VCS)
 - Version control allows you to revert a file or project to a previous version.
 - tracks modifications and who modifies
 - compares changes
 - mistakes with files can be fixed
 
### Types of Version Controls
 CVCS: Centralized Version Control System
  - Developer team collaboration on a single file or file set
  - Allows one server to store all changes and file versions
  - Eliminates the need to use all local databases
 
 DVCS: Distributed Version Control
  - Allows clients to make repository copies
  - Useful if CVCS server goes down
  - Can be placed back onto server to replace lost info
  - mirrored repositories
 
Repository - a collection of files or folders you tell Git to pay attention to. Your project.  
  * Large projects can have multiple repositories for different parts of the system

Snapshots -a saved version of a project. Commit command takes a snapshot of the file to store it. 


# Git Commands

git clone (URL of repository) -to add repository (project) 

## A C P

  **(Add)**  
   * git add (file name) -Adds staging 
 
  **(Commit)** 
   * git commit -m "your message here" *quotations necessary* -commits
 
  **(Push)**  
   * git push origin main -updates github


git status - shows us where we are

git pull -retrieves newer changes from git

### Identity Setting
  git config --global user.name "git username" (incude quotes)
  git config --global user.email "git emal" (include quotes)

### Getting Help
 * git help _command_
 * git _command_ --help
 * man git-_command_

 [Reading Source](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)


[<<<Back](README.md)