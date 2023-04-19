# Basic Overview of Git Workflow

## Making/Cloning a repository

* ```git init``` - creates a new repository in the current directory

* ```git clone url``` - clones a repository from a remote location

## Making changes

* ```git status``` - shows the status of the current repository


* ```git add``` - adds something to the staging area
  * ```git add filename``` - adds a single file in the current directory
  * ```git add .```  - adds all files in the current directory
  * ```git add -A``` - adds all files in the current directory and subdirectories
  * ```git add -u``` - adds all files that have been modified

![git_add.png](img/git_add.jpg)

* ```git commit -m "message"``` - commits the changes to the repository

### Remote Branch

* first push
  * ```git push -u origin master``` - pushes the master branch to the remote repository
  * ```git push -u origin branch_name``` - pushes the branch to the remote repository
* further pushes
  * ```git push``` - pushes the current branch to the remote repository