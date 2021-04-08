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
<br>

# Git Installation on Linux(Ubuntu)

Git is an open-source distributed version control system that is available for everyone at zero cost. It is designed to handle minor to major projects with speed and efficiency. It is developed to co-ordinate the work among programmers. The version control allows you to track and work together with your team members at the same workspace.

Git is the most common source code management (SCM) and covers more users than earlier VCS systems like SVN. Let's understand how to install Git on your Ubuntu server.

<b>Step1: Start the General OS and Package update</b>

First of all, we should start the general OS and package updates. To do so, run the below command:
```
$ sudo apt-get update
```
<b>Step2: Install Git</b>
```
$ sudo apt-get install git-core
```
<b>Step3: Confirm Git the installation</b>

To confirm the installation, press 'y' key on the editor. Now, Git is installed and ready to use. When the central installation done, first check to ensure the executable file is set up and accessible. The best way to do this is the git version command. It will be run as:
```
 $ sudo git --version
```

<b>Step4: Configure the Git for the First use</b>

Now you can start using Git on your system. You can explore many features of the version control system. To go with Git, you have to configure the initial user access process. It can be done with the git config command. Suppose I want to register a user whose user name is "javaTpoint" and email address is "Javatpoint@xyz", then it will be done as follows:

To register a username, run the below command:
```
$ git config --global user.name "javaTpoint"  
```

To register an email address for the given author, run the below command:
```
$ git config --global user.email "javatpoint@xyz" 
```
<br>
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

# Git Checkout
In Git, the term checkout is used for the act of switching between different versions of a target entity. The git checkout command is used to switch between branches in a repository. Be careful with your staged files and commits when switching between branches.
![alt text](https://static.javatpoint.com/tutorial/git/images/git-checkout.png)

The git checkout command operates upon three different entities which are files, commits, and branches. Sometimes this command can be dangerous because there is no undo option available on this command. It checks the branches and updates the files in the working directory to match the version already available in that branch, and it forwards the updates to Git to save all new commit in that branch.
### To demonstrate available branches in repository, use the below command:
```
$ git branch
```
### Now, you have the list of available branches. To switch between branches, use the below command.
```
$ git checkout <branch_name>
```
<br>
<br>
<br>

# Git Revert
In Git, the term revert is used to revert some changes. The git revert command is used to apply revert operation. It is an undo type command. However, it is not a traditional undo alternative. It does not delete any data in this process; instead, it will create a new change with the opposite effect and thereby undo the specified commit. Generally, git revert is a commit. It can be useful for tracking bugs in the project. If you want to remove something from history then git revert is a wrong choice. Moreover, we can say that git revert records some new changes that are just opposite to previously made commits. To undo the changes, run the below command:
```
$ git revert
```
<br>
<br>
<br>

# Git Remote
In Git, the term remote is concerned with the remote repository. It is a shared repository that all team members use to exchange their changes. A remote repository is stored on a code hosting service like an internal server, GitHub, Subversion, and more. In the case of a local repository, a remote typically does not provide a file tree of the project's current state; as an alternative, it only consists of the .git versioning data.

The developers can perform many operations with the remote server. These operations can be a clone, fetch, push, pull, and more. Consider the below image: 
![alt text](https://static.javatpoint.com/tutorial/git/images/git-remote.png)

### Remote checking
To check the configuration of the remote server, run the git remote command. The git remote command allows accessing the connection between remote and local. If you want to see the original existence of your cloned repository, use the git remote command. It can be used as:
```
$ git remote
```

### Git remote add
When we fetch a repository implicitly, git adds a remote for the repository. Also, we can explicitly add a remote for a repository. We can add a remote as a shot nickname or short name. To add remote as a short name, follow the below command:
```
$ git remote <tag_name> <remote URL>
```
### For knowing online directory path
```
$ git remove -v 

or

$ git remote -verbose
```
<br>
<br>
<br>

# Git Log
he advantage of a version control system is that it records changes. These records allow us to retrieve the data like commits, figuring out bugs, updates. But, all of this history will be useless if we cannot navigate it. At this point, we need the git log command.

Git log is a utility tool to review and read a history of everything that happens to a repository. Multiple options can be used with a git log to make history more specific. Generally, the git log is a record of commits. A git log contains the following data:

<br>

>1. <b>A commit hash</b>, which is a 40 character checksum data  generated by SHA (Secure Hash Algorithm) algorithm. It is a unique number.
>1. <b>Commit Author metadata:</b> The information of authors such as author name and email.
>1. <b>Commit Date metadata:</b> It's a date timestamp for the time of the commit.
>1. <b>Commit title/message:M</b> It is the overview of the commit given in the commit message.

<br>

Git log command is one of the most usual commands of git. It is the most useful command for Git. Every time you need to check the history, you have to use the git log command. The basic git log command will display the most recent commits and the status of the head. It will use as:
```
$ git log
```
The above command will display the last commits
<br>
<br>
<br>

# Git Fetch 
Git "fetch" Downloads commits, objects and refs from another repository. It fetches branches and tags from one or more repositories. It holds repositories along with the objects that are necessary to complete their histories to keep updated remote-tracking branches.
![alt text](https://static.javatpoint.com/tutorial/git/images/git-fetch.png) 

### To fetch a remote repository
```
$ git fetch <repository URL>
```
<br>

### <b>Fetch a sepecific branch</b>
We can fetch a specific branch from a repository. It will only access the element from a specific branch. See the below output:
```
$ git fetch <brancg name> <branch url>
```
<br>

### <b> To fetch all branch</b>
```
$ git fetch -all
```
<br>
<br>
<br>

# Git Pull
The term pull is used to receive data from GitHub. It fetches and merges changes from the remote server to your working directory. The git pull command is used to pull a repository.
![alt text](https://static.javatpoint.com/tutorial/git/images/git-pull.png)

Pull request is a process for a developer to notify team members that they have completed a feature. Once their feature branch is ready, the developer files a pull request via their remote server account. Pull request announces all the team members that they need to review the code and merge it into the master branch.

The below figure demonstrates how pull acts between different locations and how it is similar or dissimilar to other related commands.
![alt text](https://static.javatpoint.com/tutorial/git/images/git-pull2.png)
he pull command is used to access the changes (commits)from a remote repository to the local repository. It updates the local branches with the remote-tracking branches. Remote tracking branches are branches that have been set up to push and pull from the remote repository. Generally, it is a collection of the fetch and merges command. First, it fetches the changes from remote and combined them with the local repository.

The syntax of the git pull command is given below:
```
 $ git pull origin master
```
<br>
<br>
<br>

# Difference between Pull andd Fetch
 
|Git Fetch |Git Pull|
|:---:|:---:|
|Fetch downloads only new data from a remote repository.|Pull is used to update your current HEAD branch with the latest changes from the remote server.|
|Fetch is used to get a new view of all the things that happened in a remote repository.|Pull downloads new data and directly integrates it into your current working copy files.|
|Fetch never manipulates or spoils data.|Pull downloads the data and integrates it with the current working file.|
|It protects your code from merge conflict.|In git pull, there are more chances to create the merge conflict.|
|It is better to use git fetch command with git merge command on a pulled repository.|It is not an excellent choice to use git pull if you already pulled any repository.|

<br>
<br>
<br>

# Git Push
The push term refers to upload local repository content to a remote repository. Pushing is an act of transfer commits from your local repository to a remote repository. Pushing is capable of overwriting changes; caution should be taken when pushing.
![alt text](https://static.javatpoint.com/tutorial/git/images/git-push.png)

Moreover, we can say the push updates the remote refs with local refs. Every time you push into the repository, it is updated with some interesting changes that you made. If we do not specify the location of a repository, then it will push to default location at origin master. The "git push" command is used to push into the repository. The push command can be considered as a tool to transfer commits between local and remote repositories. The basic syntax is given below:
```
$ git push <option> [<Remote URL><branch name><refspec>...]  
```

### Git Push Origin Master
Git push origin master is a special command-line utility that specifies the remote branch and directory. When you have multiple branches and directory, then this command assists you in determining your main branch and repository.

Generally, the term origin stands for the remote repository, and master is considered as the main branch. So, the entire statement "git push origin master" pushed the local content on the master branch of the remote location.
```
$ git push origin master
```
<br>
<br>
<br>

# Git Status
The git status command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes. This command will not show any commit records or information. Mostly, it is used to display the state between Git Add and Git commit command. We can check whether the changes and files are tracked or not.

### Status when Working Tree is cleaned
Before starting with git status command, let's see how the git status looks like when there are no changes made. To check the status, open the git bash, and run the status command on your desired directory. It will run as follows:
```
$ git status
```
<br>
<br>
<br>

# Git Head
The HEAD points out the last commit in the current checkout branch. It is like a pointer to any reference. The HEAD can be understood as the "current branch." When you switch branches with 'checkout,' the HEAD is transferred to the new branch.

![alt text](https://static.javatpoint.com/tutorial/git/images/git-head.png)

The above fig shows the HEAD referencing commit-1 because of a 'checkout' was done at commit-1. When you make a new commit, it shifts to the newer commit. The git head command is used to view the status of Head with different arguments. It stores the status of Head in .git\refs\heads directory.

### Git Show Head
The git show head is used to check the status of the Head. This command will show the location of the Head.
```
$ git show HEAD
```

### Git Detached Head
GitHub keeps track of all commits or snapshots over time. If you check the 'git log' in your terminal, you can show all the previous commits up to the first commit. Detached HEAD mode allows you to discover an older state of a repository. It is a natural state in Git.
When Head doesn't point to most recent commit, such state is called detached Head. If you checkout with an older commit, it will stand the detached head condition. 
<br>
<br>
<br>

# Git Origin Master
The term "git origin master" is used in the context of a remote repository. It is used to deal with the remote repository. The term origin comes from where repository original situated and master stands for the main branch. Let's understand both of these terms in detail.
<br>
<br>

## Git Master
Master is a naming convention for Git branch. It's a default branch of Git. After cloning a project from a remote server, the resulting local repository contains only a single local branch. This branch is called a "master" branch. It means that "master" is a repository's "default" branch.

![alt text](https://static.javatpoint.com/tutorial/git/images/git-origin-master.png)
In most cases, the master is referred to as the main branch. Master branch is considered as the final view of the repo. Your local repository has its master branch that always up to date with the master of a remote repository. Do not mess with the master. If you edited the master branch of a group project, your changes will affect everyone else and very quickly there will be merge conflicts.

### Git Origin
In Git, The term origin is referred to the remote repository where you want to publish your commits. The default remote repository is called origin, although you can work with several remotes having a different name at the same time. It is said as an alias of the system.

![alt text](https://static.javatpoint.com/tutorial/git/images/git-origin-master2.png)

The origin is a short name for the remote repository that a project was initially being cloned. It is used in place of the original repository URL. Thus, it makes referencing much easier.

Origin is just a standard convention. Although it is significant to leave this convention untouched, you could ideally rename it without losing any functionality. In the following example, the URL parameter acts as an origin to the "clone" command for the cloned local repository:
```
$ git clone https://github.com/JawadulKarim/Rakib-Sir-Lab-Task.git  
```
Some commands in which the term origin and master are widely used are as follows:

>1. Git push origin master
>1. Git push origin master

Git has two types of branches called local and remote. To use git pull and git push, you have to tell your local branch that on which branch is going to operate. So, the term origin master is used to deal with a remote repository and master branch. The term push origin master is used to push the changes to the remote repository. The term pull origin master is used to access the repository from remote to local.

<br>
<br>
<br>