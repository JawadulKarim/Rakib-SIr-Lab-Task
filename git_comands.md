# What is Git? 🤔🤔🤔 
Git is an open sourced version control system which is designed to handle minor or major projects with high speed and efficiency. It is basically developed to create a virtual working enviroment for developers working at different places. i.e this version control allows developers to track and work together with team members.
<br>

<br>

## Features of Git ⚙️⚙️⚙️
>1. Open Source.
>1. Scalabity.
>1. Security.
>1. Speed.

<br>
<br>

# Git Init
The git init command is the first command that you will run on Git. The git init command is used to create a new blank repository. It is used to make an existing project as a Git project. Several Git commands run inside the repository, but init command can be run outside of the repository.

```
$ git init
```
### To create a file, run the cat or touch command as follows:
```
$ touch <file name>
```
### To add files to the repository, run the git add command as follows:
```
$ git add <file name>
```
<br>
<br>
<br>

# Git Add
The git add command is used to add file contents to the Index (Staging Area).This command updates the current content of the working tree to the staging area. It also prepares the staged content for the next commit. Every time we add or update any file in our project, it is required to forward updates to the staging area.

The git add command is a core part of Git technology. It typically adds one file at a time, but there some options are available that can add more than one file at once. he git add command can be run many times before making a commit. These all add operations can be put under one commit. The add command adds the files that are specified on command line.

### For tracking all files in local repository.........
```
$ git add -A    

or

$ git add .
```
<br>

### For tracking a particular file.........
```
$ git add <file name>
```



### For checking whether file tracked or not.............
```
$ git status
```

### To cancel tracking of a particular file........
```
$ git reset <file name>
```
<br>
<br>
<br>

# Git Commit
It is used to record the changes in the repository. It is the next command after the git add. Every commit contains the index data and the commit message. Every commit forms a parent-child relationship. When we add a file in Git, it will take place in the staging area. A commit command is used to fetch updates from the staging area to the repository. The staging and committing are co-related to each other. Staging allows us to continue in making changes to the repository, and when we want to share these changes to the version control system, committing allows us to record these changes.

Commits are the snapshots of the project. Every commit is recorded in the master branch of the repository. We can recall the commits or revert it to the older version. Two different commits will never overwrite because each commit has its own commit-id. This commit-id is a cryptographic number created by SHA (Secure Hash Algorithm) algorithm.
```
$ git commit
```
### If we wish to provide a message with every commit
```
$ git commit -m "Type message here"
```
<br>
<br>
<br>

# Git Clone
In Git, cloning is the act of making a copy of any target repository. The target repository can be remote or local. You can clone your repository from the remote repository to create a local copy on your system. Also, you can sync between the two locations.

![alt text](https://static.javatpoint.com/tutorial/git/images/git-clone.png)

###The git clone is a command-line utility which is used to make a local copy of a remote repository. It accesses the repository through a remote URL. Usually, the original repository is located on a remote server, often from a Git service like GitHub, Bitbucket, or GitLab. The remote repository URL is referred to the origin.
```
$ git clone <link address>
```

![alt address](https://static.javatpoint.com/tutorial/git/images/git-clone-2.png)
<br>
<br>
<br>
