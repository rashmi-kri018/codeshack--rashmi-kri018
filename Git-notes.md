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



# Some Essential and Basic commands

## 1. git --version 
### explaination:- This command is used to check the installed version of Git in your system.

### Example: 
###  $git --version
###  output:
###  git version 2.56.0.windows.2


## 2. git config --global user.name "your name"
##    git config --global user.email "your eamil"
##    Git config --list
### Explaination:- This command configures your Git username and email, which are used to identify the author of your commits. 

### Example:
###   $git config --global user.name "Rashmi"
###   $git config --global user.email "rkhehakhiuh57@gmamil.com"
###   $git config --list
### output: 
### Rashmi
### rkhehakhiuh57@gmamil.com


## 3. git init
### Explaination:- Initializes a new Git repository in the current directory.Git creates a hidden .git directory to store repository data and history. If your project is already a Git repository, you generally don't need to run this again.

### Example: $ git init
###  output:
###   Initialized empty Git repository in /project/.git/



## 4. git clone <Repository link>
### explaination:- : Copies an existing remote repository to your computer.

### Example: $git clone git clone https://github.com/username/project.git
### output:
###  Cloning into 'project'...
### Receiving objects: 100% ...
### Resolving deltas: 100% ...


## 5. git status
### Explaination:- Shows the current state of your working directory and staging area.

### example:- $git status
###  output:
###  On branch main
### nothing added to commit 


## 6. git add filename
##    git add .

### Explaination:- Stages changes in the staging area are ready for the next commit. 
### git add filename:- Adds a specific file's changes to the staging area so they can be included in the next commit.
### git add . :- stages multiple changes throught the current directory and its subdirectories.

### example: $git add .


## 7. git commit -m "Commit message"
### explaination: Records all staged changes in the local repository.
### Example: $git commit -m "Add README introduction"
###  output:
### [main a1b2c3d] Add README introduction
### 1 file changed, 10 insertions(+)
### create mode 100644 README.md


