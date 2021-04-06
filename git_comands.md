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
