# What Markdown can do?!
## Headlines
### Different sizes

**Also**

*Change*

~~Font~~

`Continue on the list`

+ different
1. style

--- 
can|do
---|---
such | tables

[Of course links](http://noHttp.net)

>What about quotes?

&ensp;can add smileys :smiley:

# Images in Markdown

![Конфликт](merge.jpeg)

*We can insert pictures into markdown*
## For this:
+ create a gitignore file;
+ ignore in it all jpeg;
+ paste the image in the git folder;
+ and initialize the image here, like this 

``` ![text](image name)```
+ you can add links to images, like this

``` [![text](image name)](url)```

+ the name of the picture is indicated in square brackets, in case it suddenly disappears, find it as soon as possible, like this

```[Mona Liza]```

# Now about commands in git

Git has one branch (master/main) by default. In collective work on one project, many branches are usually created, in each of which work is carried out on a specific task. After all checks, the information from the created branches is added to the master/main branch. This eliminates the eternal edits of the final document (project).

## Basic commands for working with branches

* git branch
* git branch new_branch_name
* git checkout branch_name
* git branch -d branch_name

git branch - allows you to view all created branches;

git branch new_branch_name - creates a new branch;

git checkout branch_name - switches to the specified branch;

git branch -d branch_name - deletes the selected branch.

*I should have started with this, but something went wrong...*

# Initialization local repository in git

## What will be required:
1. Create a folder on directory on PC;
2. Open this folder in VSCode;
3. And write the command in the terminal  
```git init```

 Well done!

### After, in our case, we create a file with the .md extension and again go to the terminal to save all this and write:

1. ```git add file_name.md```
2. ```git commit -m "git initialization"```

### And after each command, you need to monitor whether you press the buttons correctly, but this is already in the next chapter.

# State of the git

## After each commit, adding a file, new branch, deleting a branch, and so on, it is better to monitor the execution of commands, but how to do this? Like this:

* ```git log``` - displays a list of commits, who, when and with a comment why they did it, plus there will be a unique code for each commit;
* ```git status``` - will show the state of the git at the current moment (what file has changed, whether it is necessary to make a commit);
* ```git diff 37abv82...``` - compare the current branch with the selected one.

### And after each command, you need to monitor whether you press the buttons correctly, but this is already in the next chapter

~~вот пишешь, пишешь, а потом замечаешь что находишься в ветке мастер, а не в той которой собирался всё это писать....~~

## Well, for some reason, the most important team was not mentioned before, we fix it.

# git commit

### needed to commit the current state of the document in the current branch, followed by indexes, such as -m (comment), -a (appends file)

# Canceling operations

### A revert may be required if we made a commit too early, for example, forgetting to add some files or a comment to the commit. If you need to redo the commit, we make the necessary changes, add them to the index, and commit again by specifying --amend, like this:
`git commit --amend`

### This command uses the index to make changes to the commit. If nothing has changed since the last commit, then the state will remain exactly the same, and all we can change is the commit message.

### You can also cancel the file indexing, changes in the file.

# Working with remote repositories

## Basic commands:

+ git clone - we create a copy of the repository, which is located at the link. You can do this from the GitHub by finding the desired repository and clicking on the code button and copying the link;
![repository_on_GitHub](файл1.jpeg)
+ git pull - downloads everything from the current repository and consists of two commands: 
`git fetch` and `git merge` ;
+ git push - sends our version to an external repository (authorization on the external repository is required).