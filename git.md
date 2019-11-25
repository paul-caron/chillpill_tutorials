# ChillPill's Markdown Instructables

Proudly presents: 

![git logo](https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg)
# Git
[Git](https://git-scm.com/) is a version control system. It allows to keep track of all the steps taken during development of a program.

Files are added into the local git and changes on those files are aknowledged and recorded everytime a commit is done.

Git was created in 2005 by no other than superstar [Linus Torvalds](https://fr.m.wikipedia.org/wiki/Linus_Torvalds).

## Installation
Depending on the operation system there are different convenient ways to install git.
### Windows
On windows, the install can be downloaded directly from the git website. This is the download link and download will start automatically. [download windows git](https://git-scm.com/download/win)
### Linux
On linux, you can likely install it with your package manager. On a Debian/Ubuntu distribution :
```
sudo apt-get install git
```
or even better
```
sudo apt install git
```

## Git Commands
Here are some basic commands to get a project started.

### config
Configuration like username and email
```
git config --global user.name "Paul Caron"

git config --global user.email "chillpill@chillpillcoding.com"
```

### init
Create a new local repository
```
git init
```
### clone
Copy a repository from local repo or from remote repo, such as from [github](https://github.com/)
```
git clone /path

git clone https://somegitservice.com/user/repo
```

### add
Add file(s) for staging
```
git add filename

git add *

git add .
```

### commit
Commit changes
```
git commit -m "here you write a message about the changes"

git commit -a
```

### push
Send changes to remote repository
```
git push

git push origin master
```

### status
List info about files present in the repo.
```
git status
```

### remote
Connects to remote repository or to list currently connected repositories
```
git remote add origin master < server >

git remote -v
```

### pull
Update and merge from remote to local repository
```
git pull
```

### branch
List branches, create new branch, delete a branch
```
git branch

git branch < new branch name >

git branch -d < branch name to be deleted >
```

### merge
Merge a different branch into the active one
```
git merge < branch name >
```

### checkout
Switch to another branch
```
git checkout < branch name >
```
or create a new branch and switch to it as current working branch
```
git checkout -b < new branch name >
```

### fetch
Fetches the changes done from remote repo to local repo (without modifying local files)
```
git fetch
```
and to remove tracking references that are no longer present on the remote (prune)
```
git fetch -p
```

### reset
reset commit history
```
git reset --soft
```
reset commit history and the staged snapshot
```
git reset --mixed
```
reset commit history, the staged snapshot and the working files
```
git reset --hard
```

