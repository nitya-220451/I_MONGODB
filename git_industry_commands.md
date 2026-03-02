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


*git add .
Syntax:
git add .
Purpose:
Adds all new and modified files in the current directory (and subdirectories) to the staging area.
Screenshot:
![alt text](screenshots/gitadd.png)


*git add -p
Syntax:
git add -p <file_name>
purpose:
Allows interactive staging of changes (patch mode). You can choose specific parts (hunks) of a file to stage instead of staging the entire file.
Example:
git add -p app.js
Screenshot:
![alt text](screenshots/git_add_p.png)


*git restore
Syntax:
git restore <file_name>
Purpose
Discards changes in the working directory (restores the file to the last committed version).
Example
git restore style.css
Screenshot:
![alt text](screenshots/gitrestore.png)


*git restore --staged
Syntax
git restore --staged <file_name>
Purpose
Removes a file from the staging area but keeps the changes in the working directory.
Example
git restore --staged index.html
Screenshot:
![alt text](screenshots/gitstaged.png)


*git rm
Syntax
git rm <file_name>
Purpose
Removes a file from both the working directory and staging area, preparing the deletion for the next commit.
Example
git rm oldfile.txt
Screenshot:
![alt text](screenshots/rm.png)


5.Commit commands

*git commit
Syntax
git commit
Purpose
Creates a commit using the staged changes.
It opens the default text editor to write a commit message.
Example:
git commit
Screenshot:
![alt text](screenshots/gitcommit.png)


*git commit -m
Syntax
git commit -m "commit message"
Purpose
Creates a commit with a message directly in the command line (without opening an editor).
Screenshot:
![alt text](screenshots/commit_m.png)


*git commit --amend
Syntax
git commit --amend
Purpose
Modifies the most recent commit.
Change the commit message
Add newly staged changes to the previous commit
Example:
git commit --amend



6. Branch Management Commands
*git branch
Syntax:
git branch
Purpose:
Lists all local branches in the current repository. The active branch is marked with *
Screenshot:
Example:
git branch
![alt text](screenshots/gitbranch.png)


*git branch -a
Syntax:
git branch -a
Purpose:
Lists all branches — local and remote.
Example:
git branch -a
Screenshot:
![alt text](screenshots/git_branch_a.png)


*git branch -d
Syntax:
git branch -d <branch-name>
Purpose:
Deletes a branch safely (only if it has been merged).
Example:
git branch -d feature-login

