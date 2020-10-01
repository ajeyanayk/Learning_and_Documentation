# Git and Github documentation

#### Git - is distributed version controlled system (software) by which we can Store code individually in local system and then push it to Git Hub <br />
_Eg: In Local System (Laptop or Computer) , we generate the code and then we push the code to Git Hub._
 
**Git Hub - is web based hosting service for Git Repository. Which will take code from Local Repository and integrate all codes and make an file called master.**

1. **What is the difference between Centralized Version System and Distributed Version System ?** <br />

**Centralized Version system** will take data from Local repositories stores in one Remote Systems (Repository). once the data are moved to Remote Repository and if the Remote System fails due to some reasons , then we don't have any option to retrieve the data. 

**Distributed Version System** will take the data from Local Repositories and stores in one Remote Systems (Repository). Here the data are saved in local system and will not get deleted ,even after the data moved to Remote system. If either of repository will get deleted, then at least we can retrieve the data from one of the repositories.

Also Distributed Version System we can work in without internet connection and we can push the data when internet is restored. which is not possible in Centralised Version System as the codes are saved in Server or Remote Repository.

**Repository** : is the place, where we are store the codes or data. If we are storing the codes in Local System it is called as Local Repository. If we are storing the data in Server the it is Remote Repository.

2. **How to create Git Hub Account ?** <br />
Login to [Git hub](https://github.com/) and click on Signup button and fill the details as requested, It end with message account created successfully.

3. **How to create Git Hub Repository ?**
```Login --> Repository --> New --> Repository name --> Public /Private --> Create Repository.```

4. **How to add/ create a new file in Repository ?** <br />
```Open Repository --> add  file --> Create New File --> Type Codes -->  commit directly as Master / create new branch file--> create new file.``` <br />
Here if the file is new then select as " commit directly as Master" or If the want to add as version and to merge later, then select " create new branch file".

5. **How to look back to the previous version or previous state in Git Hub?** <br />
```Select Repository --> commits --> Select commits (version)```
 
6. **Why we need to create branch ?** <br />
because if we are not sure whether we need to add the codes /features to the Master  or not.to overcome from this we will create a branch. whenever we required in Future we just need to merge.

7. **How we can Merge two or more files ?** <br />
When we are sure the new code to be added in Master file, <br />
```Repository name -->  click on Compare & pull request```
* If the lines are conflicting both files --> ```click on pull Request --> Resolve Conflicts``` <br />
 
 Then rearrange the line as required and click on Mark as resolved -->```Commit merge -->  Merge pull request --> Confirm merge```. Once done click on the Code and then check.

8. **How can I contribute to project of which I am not a member ?**
Search for project link --> ```Select Repository --> Create New File``` ( Please note this file will not be added to Project until approval and it will create as Fork) --> type file name --> Enter the code --> propose new file --> Create Pull Request --> It checks any conflicts (Such name etc..) if there is no conflict then it allows to commit.
Once files are created the file will reach to my Repository as well as designated project pull Request-->  Merge Pull Request --> confirm merge --> will go to the repository
Please check the file before confirm. If the file is not correct, then type the comment and click on close pull request.


