# Git and GitHub command cheat sheet

**init**

Creating a local repository

$ git init

**clone**

1.Copy the project from the remote repository

$ git clone [repository_path]

2.Copy the project by specifying the name of the directory you want to create

$ git clone [repository_path] [new repository_path]

3.Copy the project to get only the latest revision

$ git clone --depth 1 [repository_path]

**branch**

Create branches

$ git branch [branch]

Display a list of branch

$ ls -ltr

Display all branches

$ git branch -a

Display the remote branch

$ git branch -r

Delete the branch

$ git branch -d [branch]

**checkout**

$ git checkout -b [branch]

**diff, status**

Display the differences of changed files

$ git diff

**Display a list of changed files**

$ git status

**add**

Register all of the files and directories to index

$ git add .

**commit**

Commit files that have been added to the index

$ git commit

**Commit a file with the commit message**

$ git commit -m "[comment]"

**Commit to add to all the changed files index (file newly added is not included)**

$ git commit -a

Modify the last commit

$ git commit --amend

**log, show**

Display the commit log

$ git log

**Display the latest commit content**

$ git show

**reset**

Cancel the last commit (the contents intact)

$ git reset --soft HEAD^

**Cancel the contents and commit of the last commit**

$ git reset --hard HEAD^

**Push**

Submit to commit the local repository to the remote repository

$ git push [remote] [branch]

**Submit to commit the master of the local repository to the master of the remote repository**

$ git push origin master

**pull-request**

Send a pull request

$ git pull-request


**Commit the file with the message of the pull request**

$ git pull-request -m "[comment]" -b defunkt:master -h mislav:feature

**merge**

Merge the branch

$ git merge [branch]

**fetch, pull**

1.Confirm the change of the remote repository

git fetch [remote]

2.Incorporate a change in the remote repository

$ git pull [remote]

**cherry-pick**

Copy the commit of another branch to the current branch

$ git cherry-pick [commit id]





