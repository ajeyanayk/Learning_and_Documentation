




Useful Links :
==============
https://dzone.com/articles/top-20-git-commands-with-examples
  2. https://stackoverflow.com/questions/25608809/git-log-p-vs-git-show-vs-git-diff#:~:text=For%20git%20diff%20this%20syntax,single%20commit%20in%20that%20range. 
3. https://dev.to/neshaz/how-to-use-git-merge-the-correctway-25pd
4. https://jonathanmh.com/how-to-create-a-git-merge-conflict/
5.https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts
6.https://www.atlassian.com/git/tutorials/cherry-pick

yet to learn
========
cherry-pick
tagging
merge conflicts
visual studio and git


GIT COMMANDS 

information
===========
git status
git log
git diff
git remote -v
git branch
git show
change info : git tag -a v1.4 -m "my version 1.4"

changing commands
==================
git add
git reset
git branch -D <NEW_BRANCH_NAME>
git reset <COMMIT ID>
git rm <FILENAME> 
git mv <FILENAME> <NEW_FILENAME>
git merge => example locally

WORKFLOW: LOCAL SIDE
=============

A. Configuration
------------------
git config --global user.name "user name"
git config --global user.email "user email id"
git config --list

B. GITHUB Repository to Local
-----------------------------
1. git clone <REPOSITORY_NAME> 
2. git checkout -b <NEW_BRANCH_NAME>
3. git add -A or git add <FILENAME>
4. git commit -m "description" #local commit into branch
5. git push -u origin <NEW_BRANCH_NAME>

C. Local to GITHUB
-----------------------
1. mkdir <REPOSITORY_NAME> #create a repository folder <REPOSITORY_NAME>
2. cd <REPOSITORY_NAME> #change into folder
3. git init #initialize 
4. create files #normal editor files
5. git add -A or git add <FILENAME> ( -A for all files)
6. git commit -m "some useful message"
7. create a repository on GITHUB
8. git remote add origin remote <repository URL>
9. git remote -v (verify )
10. git push origin master

d. update setup
----------------------
get fetch origin
git pull --rebase

USUAL SCENARIO
1. git clone latest repo
or
1. git fetch
2. git checkout -b <BRANCH_NAME>
3. work on your code, check if everything is ok with git status
4. git add -A
5. git commit -m "descripttion"
6. git pull --rebase
7. resolve any conflicts and update
8. git push