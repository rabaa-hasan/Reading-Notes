# GitHub
![GitHub](https://technologyconversations.files.wordpress.com/2015/10/github.png?w=625)
### Local Version Control
Many years ago, programmers created Local Version Control systems. A Local VCS entails one database on your hard disk that stores changes to files.

### Centralized Version Control
The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS). This system entails a single server storing all changes and file versions, which can be accessed by various clients.
### Distributed Version Control
A Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure. If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions. Also, in the event of corruption of a central database’s hard disk — with the absence of backups — all work will be lost, except for any portions on local machines.
## what is Git?
### Snapshots
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

### Local Operations
Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

### Tracking Changes
Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

### Loss of Data

Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

### States
Files in Git can reside in three main states: committed, modified and staged.

* Committed

Data is securely stored in a local database

* Modified

File has been changed but not committed to the database
* Staged

Flagged a file’s changed version to be committed in the next snapshot

![flow](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

## Download Git
In order to use Git, your computer must have it available. If you already have Git on your computer, you should make sure you have the latest version.

Git can be installed in three ways:

1. Install as a package
2. Install via another installer
3. Download and compile the source code.
## Graphical Clients
Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.

# Workflow
## Local Repository Structure
The local Git repository has three components:

* Working Directory: The actual files reside here.
* Index: The area used for staging
* Head: Points to the most recent commit
![local repo structure](https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)
## Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

* Tracked

Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

* Untracked

Untracked files were not in the last snapshot and do not currently reside in the staging area.

*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.
## The Life Cycle of File Status
1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
2. You stage the modified file.
3. Then, you commit staged changes.
![lifeCycleOfStatus](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)
# Remote Repositories
In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.

## Cloned Repositories
As mentioned earlier, for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

## Seeing Your Remotes
By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.

By using git remote -v, you can view all the remote URLs next to their corresponding short names.

