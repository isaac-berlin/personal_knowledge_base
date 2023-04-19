# Generic Git Workflow

## Clone the Repository

```git clone url``` - clones a repository from a remote location

#### Authentication

* if you are using ssh, you will need to add your public key to your account
* if you are using https, you will need to enter your username and password/authorization token

## Create a Branch

```git checkout -b branch_name``` - creates a new branch and switches to it

#### Branch Naming Conventions

* production is the only branch that should be deployed to production
* non-production branches should be named after the feature they are working on
  * prefix with your initials
  * for example, if you are working on a feature called "add login", you would name your branch ```ib_add_login```

## Switching Branches and Merging Production

```git checkout branch_name``` - switches to an existing branch

```git merge production``` - merges the production branch into the current branch

Do this before you start working on a feature. This will ensure that you are working with the latest production code.

## Committing Changes

```git add .``` - adds all changes to the staging area

```git commit -m "commit message"``` - commits the changes in the staging area

Commit messages should be descriptive and concise. They should also be in the present tense. For example, "add login" is better than "added login".

## Pushing Changes

```git push -u origin branch_name``` - pushes the changes to the remote repository and sets the upstream branch (only do this the first time you push to a branch)

```git push``` - pushes the changes to the remote repository (do this after the first time)

## Pull Requests

* create a pull request on github
* add a description of the changes you made

## Merging Changes

* merge the pull request on github
* delete the branch on github and locally

locally - ```git branch -d branch_name```

upstream - github automatically deletes the branch on the remote repository after it is merged
