## Git is a DVCS. 




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
 
 

Repository - a collection of files or folders you tell Git to pay attention to. Your project.  
  * Large projects can have multiple repositories for different parts of the system
  *


# Git Commands

git clone (URL of repository) -to add repository (project) 
 
 ## A C P
  **(Add)**  
   * git add README.md -Adds staging 
 
  **(Commit)** 
   * git commit -m "your message here" *quotations necessary* -commits
 
  **(Push)**  
   * git push origin main -updates github


 * git status - shows us where we are
 * git pull -retrieves newer changes from git
