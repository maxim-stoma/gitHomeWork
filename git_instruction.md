# GIT version control system (VCS) guide: get started

Let me advise you some simple steps to get started vcs for your work or education. Lets talk about [GIT](https://git-scm.com/ "git-scm.com") and try some examples without OS gui for local repositories. For a better experience, you can try IDE's or editors that support vcs, such as [VSC](https://code.visualstudio.com/download "VSC") from MS

![GIT](./images/git.png "git-scm.com")

## Installation and status check

* for ***Windows***: the simpliest way launch <a href=https://git-scm.com/download/win>binary installer</a>

* for ***Linux***: git is regulary default package utility, but if needed you can install it manualy. Execute in any shell you like `sudo apt/dnf install git`. Also you can visit <a href=https://git-scm.com/download/linux>Git official instruction for Linux</a>

* for ***Mac OS***: try `git --version` in shell. If there no git utility, you'll be invite to install it. Also you can invoke package manager Homebrew from shell: `brew install git` or use <a href=https://git-scm.com/download/mac>binary installer</a>

* after installation you can check your git utility status by running `git --version`

## Introducing

To work with installed VCS you must be authorized author for manage changes in your projects. This is named commits in VCS. So, on this step you have to authorize yourself in git system:

* `git config --global user.name "John Doe"` - this shell script allow you use you alias
* `git config --global user.email johndoe@example.com` - this script allow you to be authorized by email

Above is a basic configuration for built-in git utility, but you can extended this by replacing default branch naming or set your SSH connection anytime

## Create your first repository

* open your terminal for ***MacOS/Linux*** or invoke search and type `cmd` for ***Windows***

* running `mkdir myFirstRepo`

* running `cd ./myFirstRepo` 

* running `touch helloWorld.md`. You can script it in one string: `mkdir myFirstRepo; cd ./myFirstRepo; touch helloWorld.md`

* create your local repository by running `git init`

* check your git status `git status`

## Some regular commands

* `git --help` (git -h or man git) - print commands list for git
* `git version` (same git --version) - check git version
* `git init` - create a new empty repository
* `git status` - check the current status of repository
* `git add` - adding an unattracted files to git
* `git commit` - save the changes
* `git branch` - command for working with branches
* `git checkout` - switch between branches
* `git diff` - check commit difference
* `git log` - check the changelog

## Conclusion and additions

This express guide will help you to get started with git at your local machine. In the next part we will talk about remote repositories and [Git hub](https://github.com/ "github.com").

More details you can find in oficial [documentation](https://git-scm.com/doc "git-scm.com"). 

Also, I'd like to present you simple guide for markup languge [Markdown](./additions/markdown_instruction.md "markdown"). 

For the best experience I recommend you to study the [command listing](./additions/commands_list.md "command list") used for this guide preparation

# GIT version control system (VCS) guide: remote repositories and GitHub service

As i told promised, here is the second part of VCS express guide. Let's try to figure out how we can share of our projects or participate in external projects and calloborate with team online. [Git hub](https://github.com/ "github.com") is one of the most popular free online services for storing and circulating program code, managing remote repositories, sharing information and developers collaborating around the world. It's like a very advanced social network for the IT industry

## Registration

1. Registrate GitHub.com account and configure your SSH clint and IDE connection (optional)

## GIT clone

1. Create a directory on your local machine and change to it
2. Create or fork remote repository
3. Copy link (https or SSH) from GitHub and running `git clone <link>`. Or try GitHub CLI
4. Check current directory and git status

## Create remote repository and configure local repository manualy

1. Create local repository
2. Create remote repository on GitHub
2. Link local and remote repositories. See hints generated during repository creation on Github (`git remote add repository url`)
3. Send (`push`) your local repository to remote (Github)
4. Make chenges from another computer
5. Recieve (`pull`) actual stage from remote repository 

## Collective work with repositories (using fork)

1. Make fork of target repository on GitHub
2. Clone it to your local machine
3. Prepare changes in separate new branch
4. Commit and push to your remote (just forked) repository
5. Create pull request and send it to repository origin owner

<hr>

### Feedback

For any questions and suggestions, do not hesitate to contact me by e-mail: Berezhnoy_aa@mail.ru or write to Telegram @Berezhnoy_Sasha