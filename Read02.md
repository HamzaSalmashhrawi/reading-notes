#### Student name: Hamza S Almashhrawi.
# INTRODUCTION
## Prerequisites
#### Before beginning this tutorial, it is highly recommended that you have a solid understanding of the Terminal (for Mac) or Command Line (for Windows and Linux). In order to explain Git, we have to first explain various aspects of Version Control.
## Version Control
#### Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes. By utilizing a Version Control System (VCS), mistakes with files can easily be rectified.
## Local Version Control
#### Many years ago, programmers created Local Version Control systems. A Local VCS entails one database on your hard disk that stores changes to files.
## Centralized Version Control
#### The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS). This system entails a single server storing all changes and file versions, which can be accessed by various clients. This streamlined the collaboration process (by eliminating the need to involve all local databases), allowed programmers to have more knowledge of team members’ activities with certain files, and gave administrators much more control over divvying up revision privileges.
## Distributed Version Control
#### A Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure. If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions. Also, in the event of corruption of a central database’s hard disk — with the absence of backups — all work will be lost, except for any portions on local machines.To prevent this type of catastrophic loss, a DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information. Because the DVCS allows for multiple mirrored repositories, programmers working in teams can collaborate with each other in various ways to complete a joint project, which enables the use of various simultaneous workflows.

# So, what is Git?
## Snapshots
#### Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project called commit Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
## Local Operations
#### Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

## Tracking Changes
#### Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

## Loss of Data
#### Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.
#### Flagged a file’s changed version to be committed in the next snapshot
![gitpicc](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

# Getting Started
## Download Git
### In order to use Git, your computer must have it available. If you already have Git on your computer, you should make sure you have the latest version.

## Git can be installed in three ways:

1. Install as a package
2. Install via another installer
3. Download and compile the source code.

# Windows

## Git Website

### You can download Git by visiting this link and following the posted directions:

[gitwindowsdownload](http://git-scm.com/download/win)

### GitHub

### Install Git as part of the GitHub for Windows install:

[gitinstall](http://windows.github.com)

## Graphical Clients

#### Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.
#### GUI Clients
#### You can access a variety of GUI clients for Mac, Windows, and Linux via the following link:

[GUIclients](https://git-scm.com/downloads/guis)

## Initial Customization
#### After making sure Git has been installed, you should perform some customization steps, which should only need to be completed once on any machine. To change settings, you can repeat these steps.
### **Configuration of Variables**
#### An inherent Git tool called git config allows the setting of configuration variables that control aspects of Git’s operation and look.
**___________________________________________________________________________________________**
# Setting up a Git Repository
## Importing
#### To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

#### 1. Switch to the target project’s directory
#### Example:

 $ cd test (cd = change directory)

#### 2. Use the git init command
 $ git init
 
#### 3. To start tracking these repository files, perform an initial commit by typing the following:
* $ git add *.c
* $ git add LICENSE
* $ git commit -m “any message here”

# Workflow
## Local Repository Structure
## The local Git repository has three components:

1. Working Directory: The actual files reside here.
2. Index: The area used for staging
3. Head: Points to the most recent commit

![headpoints](https://blog.udemy.com/wp-content/uploads/2015/08/image036-768x228.png)

## Saving Changes
### All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

### **Tracked**

### Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

### **Untracked**

### Untracked files were not in the last snapshot and do not currently reside in the staging area.

### After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

## The Life Cycle of File Status
### 1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
### 2. You stage the modified file.
### 3. Then, you commit staged changes.
![untracked](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

## Stashing Changes
#### When you are not ready to commit changes but do not want to lose them either, git stash is a great option. This command temporarily removes changes and hides them, giving you a clean working directory. When you are ready to continue working on the changes, simply use the git stash apply command to retrieve the hidden changes.




