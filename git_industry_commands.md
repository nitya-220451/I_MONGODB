1. Git configuration commands
*git config --global username
##syntax
git config --global user.name "Nitya Sri"
**Screenshot
![alt text](screenshots/username.png)

*git config --global user.email
##syntax
git config --global user.email "n220451@rguktn.ac.in"
**Screenshot
![alt text](screenshots/email.png)

*git config --list
##syntax
git config --list
**Screenshot
![alt text](screenshots/list.png)

*git config --unset
##syntax
git config --unset user.name
**Screenshot
![alt text](screenshots/unset.png)

2.Repository setup commands

*git init
##syntax
git init
**Screenshot
![alt text](screenshots/init.png)

*git clone
##sytax
git clone <repository_url>
Example:
git clone https://github.com/nitya-220451/I_MONGODB.git
**Screenshot
![alt text](screenshots/clone.png)


*git clone --branch
##syntax
git clone --branch <branch-name> <repository_url>
Example:
git clone --branch feature1 https://github.com/nitya-220451/I_MONGODB.git
**Screenshot
![alt text](screenshots/clonebranch.png)


*git clone --depth
##syntax
git clone --depth <number>  <repository_url>
Example:
git clone --depth 1  https://github.com/nitya-220451/I_MONGODB.git
**Screenshot
![alt text](screenshots/clonedepth.png)

3.Repository status & Inspection

*git status
purpose:shows the current state of the repository.
Example:
git status
**Screenshot
![alt text](screenshots/status.png)

*git log
Syntax:
git log
purpose:Displays the complete commit history of the repository including commit id,author,date,commit message
**Screenshot
![alt text](screenshots/gitlog.png)


*git log --oneline
syntax:
*git log --oneline
purpose:shows the commit history in a short single-line format
**Screenshot
![alt text](screenshots/gitoneline.png)

*git log --graph
Syntax:
*git log --graph
purpose:Displays the commit history in a graphical tree structure showing branches and merges
**Screenshot
![alt text](screenshots/gitgraph.png)

*git show
Synatx:git show <commit-id>
purpose:shows detailed information about specific commit,including the changes made
Example: git show a34f567
Screenshot:
![alt text](screenshots/gitshow.png)

*git diff
Syntax: git diff
purpose:shows the difference between the working directory and the staging area
Exapmle:git diff
Screenshot:
![alt text](screenshots/gitdiff.png)

*git diff --staged
Syntax
git diff --staged
purpose:shows changes between the staging are and the last commit
Example:
git add index.php
git diff --staged
Screenshot:
![alt text](screenshots/gitdiffstaged.png)


*git blame
Syntax:git blame <file_name>
purpose:git blame shows who last modified each line of a file and in which commit.
It helps track the author responsible for each line of code.
Example:
git blame index.php
Screenshot:
![alt text](screenshots/gitblame.png)


*git reflog
syntax:git reflog
git reflog shows the history of all HEAD movements in the repository, including:
commits
resets
checkouts
merges
It helps recover lost commits or branches.
Screenshot:
![alt text](screenshots/gitreflog.png)

*git shortlog
Syntax:git shortlog
purpose:git shortlog displays a summary of commits grouped by author.
Screenshot:
![alt text](screenshots/gitshort.png)

4.File tracking commands

*git add
Syntax:git add <file_name>
purpose:Adds a specific file to the staging area so it will be included in the next commit.
Example:
git add index.html
Screenshot:
![alt text](screenshots/add.png)