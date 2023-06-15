# README

This is a quick demo and practice for basic Git commands.

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#new-repo">New Repository</a>
    </li>
    <li>
      <a href="#new-branch">New Branches</a>
    </li>
    <li><a href="#add-commit">Add and Commit</a>
    </li>
    <li><a href="#update-local">Update Local Branch</a>
    </li>
    <li><a href="#history">History</a>
    </li>
    <li><a href="#next">What's Next?</a>
    </li>
  </ol>
</details>


<a name="new-repo"></a>
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


<a name="new-branch"></a>
## 2. New Branches
A new branch can be created with command: ```git branch <branch-name>```. Then you may switch to the new branch using ```git checkout <branch-name>```. 
Creating a new branch allows you to work on changes without affecting the main code, enabling parallel development and collaboration. It provides a dedicated space for developing features, trying out new ideas, and reviewing code before merging it into the main branch.


<a name="add-commit"></a>
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


<a name="update-local"></a>
## 4. Update Local Branch
The `git pull` command is used to update your local repository with the latest changes from the remote repository. It's a good idea to pull regularly on the branches you are working on locally. It combines the `git fetch` command (which retrieves the latest changes from the remote repository) and the `git merge` command (which incorporates those changes into your local branch).

These are some common usages: 
1. `git pull --rebase`: Update your local branch with the latest remote commits while rewriting your local commits to occur after the new remote commits, avoiding a merge commit
2. `git pull --force`: Occasionally, you may encounter conflicts that cannot be automatically resolved by Git. You can forcefully overwrite your local changes with the latest changes from the remote repository. Be cautious when using this option, as it discards your local commits irreversibly
3. `git pull --all`: Fetch all remotes - this can be helpful when you want to synchronize all branches with their respective remote counterparts
4. `git pull --prune`: Remove deleted remote tracking branches


<a name="history"></a>
## 5. History
You may check all the changes made using the command `git log`, which displays a list of commits to the repository. There are many options and parameters to play around with when displaying the entries, for example:
```
git log --pretty=oneline --max-count=2
git log --pretty=oneline --since='5 minutes ago'
git log --pretty=oneline --until='5 minutes ago'
git log --pretty=oneline --author=<your name>
git log --pretty=oneline --all
git log --all --pretty=format:"%h %cd %s (%an)" --since='7 days ago'
```


<a name="next"></a>
## 6. What's Next?
Here are some suggestions for further exploring additional features:

1. **Collaborate**: Invite collaborators and leverage pull requests for code review
2. **Branching**: Explore strategies such as GitFlow or GitHub Flow to optimize workflow
3. **GitHub Actions**: Automate processes using GitHub Actions to streamline development workflow
4. **Issue Tracking**: Utilize GitHub's issue tracking system for effective task management and project organization
5. **Documentation**: Create comprehensive README files and use GitHub's wiki feature
6. **Open-Source Contributions**: Contribute to open-source projects by forking and submitting pull requests





