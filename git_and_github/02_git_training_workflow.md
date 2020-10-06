<h1 align="center">Git Working flow</h1>

![git_working_flow](./images/git_workflow.png)

<h4>These are basic commands of Git, when we want to know the information of current branch</h4>

* git status - Which shows the files which have to be commited
* git log - which lists the history(log) of current branch 
* git diff - which shows the difference between two branches (staging area and latest version )
* git remote -v  - to connect local repostory to  remote server
* git branch -  which lists branches in current repository
* git show - 
* change info : git tag -a v1.4 -m "my version 1.4" - to check the tags for specified commit

<h4>These commands are used, when we want to change any content in branch or in files</h4>

* git add - to add the file to staging area 
* git reset - to remove the file from staging area
* git branch -D <NEW_BRANCH_NAME> - to delete branch in repository
* git reset <COMMIT ID> - to reset the file which are already commited
* git rm <FILENAME>  to delete file current directory
* git mv <FILENAME> <NEW_FILENAME> - - to rename file name
* git merge - to merge two branch 


**Sequence to be followed in Local machine to be get updated in GITHUB**

* GITHUB configuration in Local machine

* *git config --global user.name "user name"* - commands to used to set user name for git
* *git config --global user.email "user email id"* - commands to set email address
* *git config --list* - which lists the configured contents

* Steps for movement of files if the repositories are already created in GITHUB

1. *git clone <REPOSITORY_NAME>* - command is used to pull the data from perticular repository
2. *git checkout -b <NEW_BRANCH_NAME>* - to switch from one branch to another
3. *git add -A or git add <FILENAME>* - to add a new file to branch
4. *git commit -m "description"* - to commit a new/updated file to branch
5. *git push -u origin <NEW_BRANCH_NAME>* - moving a file or set of files in branch to github

* Steps to create a new Repository in local machine and movement of files

1. mkdir <REPOSITORY_NAME> - create a folder in local machine with Reposity name
2. cd <REPOSITORY_NAME> - change into folder
3. git init - which initialize a new repository
4. create files #normal editor files - 
5. git add -A or git add <FILENAME> ( -A for all files) - add the file to staging area
6. git commit -m "some useful message" - to commit a new/updated file to branch
7. create a repository on GITHUB - create a Folder in GITHUB
8. git remote add origin remote <repository URL> - to connect GITHUB from local machine
9. git remote -v (verify ) - to verify whether local machine is in connection with GITHUB
10. git push origin master - to move file/files to GITHUB

<h4>update setup</h4>

* get fetch origin
* git pull --rebase

* steps to be followed some of unsusual scenarios(need to merge file to master to test in local system etc.)
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

Useful Links :
==============
1. https://dzone.com/articles/top-20-git-commands-with-examples
2. https://stackoverflow.com/questions/25608809/git-log-p-vs-git-show-vs-git-diff#:~:text=For%20git%20diff%20this%20syntax,single%20commit%20in%20that%20range. 
3. https://dev.to/neshaz/how-to-use-git-merge-the-correctway-25pd
4. https://jonathanmh.com/how-to-create-a-git-merge-conflict/
5. https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts
6. https://www.atlassian.com/git/tutorials/cherry-pick