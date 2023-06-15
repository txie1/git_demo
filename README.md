# README

This is a github demo!

### 1. Clone the Repository
Forking allows you to create a personal copy of the repository, while cloning creates a local copy on your computer. The link to the repository may be obtained through the green button "code" and you may use the Git command: ```git clone <repository-link>```

### 2. New Branches
A new branch can be created with command: ```git branch <branch-name>```. Then you may switch to the new branch using ```git checkout <branch-name>```. 

### 3. Add and Commit
Check the status of your changes using comand ```git status```, and add the modified files with ```add <file1> <file2> ...``` or simply ```add .``` to add all of the files. Check the status again to ensure all changes are staged ```git status```. Then commit the changes to your branch using ```git commit -m "updaded readme"```.

If you forgot the add the commit message and see the following:

```
|
# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
# On branch master
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	modified:   hello.html
#
```
To exit, insert your "commit message" on the first line. Then press "esc", type ":wq" and then Enter.


Push the changes onto github using ```git push```.




