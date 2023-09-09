![Git_logo](logo.png)

# Git instruction
This instruction is recomended for beginners who start using Git appication.
## Git commands
* git init
* git commit 
* git status
* git log
* git checkout
* git diff
* git branch 
* git branch branch_name
* git merge branch_name
* git log graph
* git clone
* git pull
* git push

**Git init**. This command *creates an empty Git repository* - basically a .git directory with subdirectories for objects , refs/heads , refs/tags , and template files.

**Git commit**. The git commit command *creates a commit, which is like a snapshot of your repository*. These commits are snapshots of your entire repository at specific times.

**Git status**. The git status command *displays the state of the working directory* and the staging area.

**Git log**. The git log command is used to *view the history of committed changes* within a Git repository.

**Git checkout**. The git checkout command *lets you navigate between the branches* created by git branch.

**Git diff**. The git diff *lists out the changes* between your current working directory and your staging area.

**Git branch**. *List all of the branches* in your repository.

**Git branch branch_name**. *Create a new branch* called ＜branch＞. ***This does not check out the new branch***.

**Git merge branch_name**. The git merge command *lets you take the independent lines* of development created by git branch and *integrate them into a single branch*.

**Git log grahp**. The git log graph command *creates a graphic overview* of how a developer's various development pipelines have branched and merged over time.

**Git clone**. *Clones a repository into a newly created directory*, creates remote-tracking branches for each branch in the cloned repository, and creates and checks out an initial branch that is forked from the cloned repository’s currently active branch.

**Git pull**. The git pull command *runs git fetch* with the given parameters and then depending on configuration options or command line flags, *will call either git rebase or git merge to reconcile diverging branches*.

**Git push**. The git push command is used to *upload local repository content to a remote repository*.

**! Sometimes conflicts happen, so you need to resolve them using some options under the lines contradicting !**

See here: ![conflict image](Git_conflict.jpg)

# Remote repository
**To be able to collaborate on any Git project, you need to know how to manage your remote repositories. Remote repositories are versions of your project that are hosted on the Internet or network somewhere. You can have several of them, each of which generally is either read-only or read/write for you. Collaborating with others involves managing these remote repositories and pushing and pulling data to and from them when you need to share work. Managing remote repositories includes knowing how to add remote repositories, remove remotes that are no longer valid, manage various remote branches and define them as being tracked or not, and more. In this section, we’ll cover some of these remote-management skills.**

That's the way it works:
![remote repository algorithm](basic-remote-workflow.png)



