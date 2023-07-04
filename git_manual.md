# GIT manual
---

#NEW SHINY INSTRUCTIONS FOR Homework_3

## git clone
This command is used for downloading the latest version of a remote project and copying it to the selected location on the local machine. It looks like this:
_git clone **repository url**_

To clone a specific branch, you can use
_git clone **repository url** -b **branch name**_

##  git push
Git push will push the locally committed changes to the remote branch. If the branch is already remotely tracked, simply use it like this (with no parameters):
_git push_

If the branch is not yet tracked, and only resides on the local machine, you need to run the command like this:
_git push --set-upstream **remote branch branch name**_
_git push --set-upstream origin **branch name**_

## git pull
Using git pull will fetch all the changes from the remote repository and merge any remote changes in the current local branch.
_git pull_

## pull request
1. Before you create a pull request, you'll need to push changes to a branch on GitHub.
    * Save and commit any changes on your local branch. For more information
    * Push your local commits to the remote repository. For more information
    * Publish your current branch to GitHub. For more information

2. Click Preview Pull Request. GitHub Desktop will open a preview dialog showing the diff of the changes between your current branch and the base branch.
3. Confirm that the branch in the base: dropdown menu is the branch where you want to merge your changes.
4. Click Create Pull Request.
5. Type a title and description for your pull request.
---

## how to install git
1. Begin studying on the GeekBrains educational platform in 2022
2. Complete Python course, begin to learn Git
3. Install and setup VS Code and Git
4. Drop out because of
    * war
    * life changing circumstances
    * 2yo daughter
    * _I hate IT_ thoughts

....

19. Forget everything 

....

32. Pull yourself together
33. Make a descision to go for Product Manager
34. Begin to study again
35. Look and your PC
36. VS Code and Git are already there!!!

...

PROFIT!

## git init
This is the command you need to use if you want to start a new empty repository or to reinitialize an existing one in the project root. It will create a .git directory with its subdirectories. It should look like this:
_git init_

## git add
This is the command you need to use to stage changed files. You can stage individual files:
_git add **file path**_

## git commit
This one is probably the most used Git command. After changes are done locally, you can save them by “committing” them. A commit is like local a snapshot of the current state of the branch, to which you can always come back. To create a new commit, type this command in Git Bash:
_git commit -m **"commit message"**_

## git branch
Using git branch will list all the branches of the repository:
_git branch_
Or you can use it to create a new branch, without checking it out:
_git branch **new branch**_

## git checkout
You can use the checkout command to switch the branch that you are currently working on.
_git checkout **branch name**_
