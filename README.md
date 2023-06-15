# README

This is a github demo!

## 1. New Repository

Get started in an empty working directory and create an empty directory named `hello`, then create a `hello.html` file in it with the following contents:

```
mkdir hello
cd hello
touch hello.html
```
Run `git init` to create a git repo from that directory. Then add the first page to repo:

```
git add hello.html
git commit -m "First Commit"
```

You may also work with an existing repository. Forking allows you to create a personal copy of the repository, while cloning creates a local copy on your computer. The link to the repository may be obtained through the green "_Code_" button and you may use the Git command: ```git clone <repository-link>```

## 2. New Branches
A new branch can be created with command: ```git branch <branch-name>```. Then you may switch to the new branch using ```git checkout <branch-name>```. 
Creating a new branch allows you to work on changes without affecting the main code, enabling parallel development and collaboration. It provides a dedicated space for developing features, trying out new ideas, and reviewing code before merging it into the main branch.



## 3. Add and Commit
After making changes you may check the status using command ```git status```, and add the modified files with ```add <file1> <file2> ...``` or simply ```add .``` to add all of the files. Check the status again to ensure all changes are staged ```git status```. Then commit the changes to your branch using ```git commit -m "updaded readme"```.

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


Push the changes onto Github using ```git push```.

## 4. History
You may check all the changes made using the command `git log`, which displays a list of commits to the repository. There are many options and parameters to play around with when displaying the entries, for example:
```
git log --pretty=oneline --max-count=2
git log --pretty=oneline --since='5 minutes ago'
git log --pretty=oneline --until='5 minutes ago'
git log --pretty=oneline --author=<your name>
git log --pretty=oneline --all
git log --all --pretty=format:"%h %cd %s (%an)" --since='7 days ago'
```





