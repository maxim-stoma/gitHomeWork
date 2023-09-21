# Git instructions

### What is Git?

**Git** is the console utility for control and lead history of changes files in your project.

 With Git you can roll back your project to older version, compare, analyze or drain your changes to the repository. 
 ### What is repository?

 **Repository** is a storage of your code and change's history. Git work in local and all your repositories  save in specific folders on your hard drive. 

 Also you can save your repositories on the internet. Typically? three services used for this:
 
 1. [**GitHub**](https://github.com/) 
 2. [**Bitbucket**](https://bitbucket.org/)
 3. [**GitLab**](https://gitlab.com/)

 Each save point of your project is called a "*commit*". Each commit has hach (specific id) and comment. A branch assembled from such commits.

## **Installation:**

* Windows. Follow [**this link**](https://git-scm.com/download/win), select one for your OS (32 or 64 bit), download and install.

* For Mac OS. Open a terminal and write:
```
#If Homebrew is installed
brew install git

#If not, then enter this command. 
git --version

#After this, a window will appear asking you to install Command Line Tools (CLT).
#We agree and wait for installation. Install git along with CLT
```
* Linux. Open a terminal and enter the following command:
```
# Debian or Ubuntu
sudo apt install git

# CentOS
sudo yum install git    
```
All done, now you can work with Git!

## Start work with Git / Setting up
### Setting up

You have installed Git and can use it. Let's now configure it so that when you create a commit, the author who created it is indicated.

Open a terminal (Linux and MacOS) or console (Windows) and enter the following commands.
```
#Set a name for your user
#Instead of <your_name> you can enter, for example, Grisha_Popov
#Leave the quotes

git config --global user.name "<your_name>"

#Now let's set the email. The principle is the same.

git config --global user.email "<@email.com>"
```
**Creating a repository:**

Now you are ready to work with Git locally on your computer.

Let's create our first repository. To do this, go to your project folder.

```
#Create the project's folder

cd <path_to_your_project>

#git initialization

git init
```

## Working with a local repository

So, we installation git, we setting up git? craete project's folder, create local repository, and what now?

Now, you can develop your project with your friands, so this is exactly why git was invented.

The main function of Git is that Git allows parallel development by branching versions of the application.

Create new branch:

**git branch _branch name_**

Now you have made a new branch

Delete branch:

**git branch -d/-D _branch_name_**

Switch between branches:

**git checkout _branch_name_**

Once you have added all the necessary code to the branch, you need to add all existing files to the commit, this is done using the **git add file_name** command

And now you can do your first commit:

**git commit -am "commit_name"**

When you have finished developing a branch, you can merge that branch into the master branch (Master branch is the master branch), you can do this using the command:

**git merge branch_name**

you can display the project's change history using the command:

**git log**

Or in graph:

**git log --praph**

### Conflicts

Conflicts can arise when merging branches if there are different versions of the same piece of code. If there is a conflict, the system itself will warn you and allow you to choose which of the code options to merge with the branch.

![](3.jpg)

Don’t be afraid if such an error appears, this is the very conflict.

![](1.jpg)

The red line marks the lists of what you can do. Arrows indicate options proposed by different branches.

![](2.jpg)

In our case we will choose "Accept incoming Change"

## Remote repositories



## Basic Commands
git init 
git status 
git branch 
git branch name_branch 
git chechout name_branch 
git branch -d/-D name_branch 
git log 
git log --graph 
git commit -am "commit_name"

## Additional commands 

git config --global user.name "<your_name>"

git config --global user.email "<@email.com>"

git --version 
