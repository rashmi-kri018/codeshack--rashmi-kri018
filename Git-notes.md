#   -------------GIT AND GITHUB--------------------

# what is GIT?
### GIT is a free , open source version control system that tracks the changes made to file in a project over time and return earlier version when necessary.
### With GIT, you can record changes as commits and use your project history to recover earlier versions.


# Why git is used?
### GIT is used because it helps:
### --> Track changes in code.
### --> Enable collaboration among developers.
### --> Maintain different version of a project.
### --> Provides a backup of the code.
### --> Make it easy to revert to previous versions.


# What is GITHUB?
### GITHUB is an online(web-based) platform that . It allows developers to hosts Git repositories,store code online, share projects, review changes, and collaborate with other developers.

# Git vs GitHub ?
### Git:- Git is a version control system which can work locally on your computer/PC and track changes.

### GitHub:- It is a cloud platform that host Git repositories and provide feature like collaboration, pull requests , issues and code review.

# What is a Repository ?
### A repository is a storage space where your project files and their history are kept. It contains all the versions of your project and helps in version control.
### Repositories are classified into two types:
###     1. Local Repository --> It is stored on your own computer.
###     2. Remote Repository --> It is stored on a remote server like GitHub, GitLab, etc.


# ==> Command-Line Interface(CLI):
### --> So basically To interact with Git , we use some commands through a command-line interface(CLI). CLI allows us to communicate with the computer by typing commands instead of using graphical buttons and menus.
### --> some commonly used command-line environment are GitBash, Terminal and powershell.



# What is working directory, Staging area, and Commit?
 ### Working directory --> It is tht current folder where we make changes to our file.

 ### Staging Area --> It is a temporary area were we keep the changes that will be included in the next commit.

 ### Commit --> It is a snapshot of the project at a particular point in time.



# what is .git?
### The .git folder is a hidden directory that stores the information Git needs to track and manage your project. It is created when you initialize a Git repository using git init or clone a repository using git clone.
### .git/ stores Git's internal information, including commit history, branch information, and repository configuration.


# Simple Git workflow
###         Working Directory
###              ⬇️ git add
###         staging Area
###              ⬇️ git commit
###         Local Repository


# What is Branch in Git?
### A branch is an independent line of development in a Git repository that allows you to work on new features or make changes without directly changing the work on another branch.
### Think of a branch as a separate workspace for developing a feature.


# Important branch commands
### Command          	    Purpose
### git branch	             Lists local branches
### git branch feature	     Creates a branch named feature
### git switch feature	     Switches to an existing branch
### git switch -c feature	 Creates and switches to a branch
### git merge feature    	 Merges the named branch into your current branch
### git branch -d feature	 Deletes a branch when Git considers it safe to delete



# What is Branching in Git?
### Branching is the process of creating and working on separate lines of development within the same Git repository.
### It allows developers to work on new features, fix bugs, or experiment with changes without directly affecting the main branch.


# Why is branching important?
### Parallel development: Multiple developers can work on different features.
### Isolation: Feature work stays separate from the main line of development.
### Experimentation: You can try changes without immediately incorporating them into main.
### Collaboration: Teams can review changes before merging them.
### Bug fixing: Developers can work on fixes independently.

# Branch vs. branching
### A branch is the separate line of development; branching is the process of creating and using it.



# Some Essential and Basic commands

## 1. git --version 
### explanation:- This command is used to check the installed version of Git in your system.

### Example: 
###  $git --version
###  output:
###  git version 2.56.0.windows.2


## 2. git config --global user.name "your name"
##    git config --global user.email "your eamil"
##    Git config --list
### Explanation:- This command configures your Git username and email, which are used to identify the author of your commits. 

### Example:
###   $git config --global user.name "Rashmi"
###   $git config --global user.email "rkhehakhiuh57@gmamil.com"
###   $git config --list
### output: 
### Rashmi
### rkhehakhiuh57@gmamil.com


## 3. git init
### Explanation:- Initializes a new Git repository in the current directory.Git creates a hidden .git directory to store repository data and history. If your project is already a Git repository, you generally don't need to run this again.

### Example: $ git init
###  output:
###   Initialized empty Git repository in /project/.git/



## 4. git clone Repository link
### explanation:- : Copies an existing remote repository to your computer.

### Example: $git clone git clone https://github.com/username/project.git
### output:
###  Cloning into 'project'...
### Receiving objects: 100% ...
### Resolving deltas: 100% ...


## 5. git status
### Explanation:- Shows the current state of your working directory and staging area.

### example:- $git status
###  output:
###  On branch main
### nothing added to commit 


## 6. git add filename
##    git add .
### Explaination:- Stages changes in the staging area are ready for the next commit. 
### git add filename:- Adds a specific file's changes to the staging area so they can be included in the next commit.
### git add . :- stages multiple changes throught the current directory and its subdirectories.


## 7. git commit -m "Commit message"
### explanation: Records all staged changes in the local repository.
### Example: $git commit -m "Add README introduction"
###  output:
### [main a1b2c3d] Add README introduction
### 1 file changed, 10 insertions(+)
### create mode 100644 README.md


## 8. git log
### explanation:- This command is used to display the history in detailed including commit IDs, authors, dates, and commit message.

### Example:- $git log
### output: 
### commit a1b2345678
### Author: Rashmi <rashmi@example.com>
### Date:   Wed Oct 14 20:30:00 2026 +0530
###    Add README introduction
### commit b2c3d4e678
### Author: Rashmi <rashmi@example.com>
### Date:   Wed Oct 14 19:45:00 2026 +0530
###  Create developer handbook


## 9.git log --oneline
### explanation: This command is used to display all the history in concised or in compact form.

### example:- $git log --oneline
### output:
### a1b2c3d Add README introduction
### b2c3d4e Create developer handbook

## 10.git diff
### explanation:- This command used to see the differences between versions of files. It helps you understand what lines you have added, modified, or removed.This command normally shows the differences between your working directory and the staging area. In simple words, it shows changes you have made but have not staged using git add.

### example: $git diff
### your original file contains:
### # Git Handbook
### This handbook explains Git basics.
### after editing in the original file , then using git diff command
### -This handbook explains Git basics.(the old line that was removed or replaced)
### +This handbook explains Git and GitHub basics. (The new line that was added or used to replace the old line)


## 11. git branch
### explanation:- This command is used to display the current branch of your current directory.

### example:- $git branch
### output: * main
### The * indicates the currently selected branch


## 12. git checkout -b branch-name
### Explanation: This command is used to create a new branch and switching to that branch from the main branch.

### Example: $git checkout -b feature-branch
### output: Switched to a new branch 'feature-branch'


## 13.git switch branch-name
### explanation:- This command  is used to switch to an existing branches.

## example: $git switch feature-branch
## output: Switched to branch 'feature-branch'



## 14. git remote add origin repository-link
### explanation:- This command is used to connects your local repository to remote repository, usually hosted on GitHub.

### example:- $ git remote add origin https://github.com/your-username/GitHub-Repository-name 


##  15. git remote -v
### Explanation:- This command displays the remote repositories connected to your local Git repository, along with their URLs.
### git remote manages remote repository connections.
### -v stands for verbose, meaning it displays additional details, including the URLs.

### example: $git remote -v
### output:-
###  origin  https://github.com/your-username/GitHub-repository-name (fetch)
### origin  https://github.com/your-username/GitHub-repository-name (push)

## fetch --> fetch means checking for and downloading new Git information from the remote repository to your local repository, without automatically merging those changes into your current branch.

## push --> push means uploading your local commits to the remote repository on GitHub.


## 16.git push origin main
##    git push -u origin name
### explanation:- Both commands upload your local commits to a remote repository, usually GitHub. The main difference is that -u sets up an upstream connection, making future pushes easier.

### example: $git push origin main
### --> You have committed changes on your local main branch and want to upload them to GitHub's main branch.
### example: git push -u origin feature-branch
### --> feature-branch — specifies the branch to push
### --> After this succeeds, Git remembers which remote branch your local branch tracks. When you're on that branch, you can generally use:
### $git push
### --> instead of specifying the remote and branch every time.


## 17.git pull repository-name branch-name
### explaination:-  git pull is a Git command that fetches changes from a remote repository and integrates them into the current local branch.

### example:- git pull origin main
### --> git	Runs a Git command.
### pull	Fetches remote changes and integrates them.
### origin	The name of the remote repository.
### main	The remote branch you want to pull from.




# Other Useful commands
## mkdir folder-name --> This command is used to make or create a new directory.

## cd folder-name --> The cd command means change directory. It lets you move into another folder.

## pwd --> The pwd commands shows your current directory.

## ls --> The ls command list files and folders in the current directory.

## ls -a --> This commmand is used to display all files and folders , including hidden files like .git .

## cd .. --> This command helps you to move from current directory to the previous one.

## 
