# Git-Notes by @rudrakshkarpe 
---


## Deletions Commands

### Deleting a .git folder from a repo
- rm -rf .git 

### To add all changes to the staging area
- git add --a 

## Git ignore commands
- touch .gitignore
- error.log
- *.log
- dir/
- /dir/ to track only outer dir it'll skip the inner one
- git by defaultly ignores the blank directories

## Comparison commands

### To compare the working  directory and staging area
- git diff 

- git diff --staged

## Commit cmmands
- git commit -a -m "your comment"
- This will commit all the tracked files untracked file needs to be added specially
- git commit --amend   to make changes in the commit

## Basic Commands 

- git rm file.txt --> remove
- git mv file.txt file_01.txt  to rename files

## Untracking files

- git rm --cached db.accdb 

## Log commands

### To check commits + files deleted
- git log -p  

### To check specific commits
- git log -3 or -2 

### to check individual commits
- git log -p -1  

### To check more specific on commits
- git log --stat  

- git log --pretty=oneline
- git log --pretty=short
- git log --pretty=full
- git log --since=2.days  filter according to time
- git log --since=2.year/months/years
- git log pretty=format:"%h --%an or ae"



## Recovery commands

### To remove any file from staging area
- git restore --staged  

### To checkout to the previous commit
- git checkout --filename.txt 

### All the changes to vanish and move to the previous commit as a clean tree
- git checkout -f  


## Remote comamnds 

### To list down the remotes
- git remote

### To add new remote
- git remote add origin git@github.com:rudrakshkarpe/repositoryname.git


- git remote -v

## SSH Key generation commands

- ssh-keygen -t rsa 4096 -C "rudraksh.karpe@gmail.com"

- eval $(ssh-agent -s)

- ssh-add ~/.ssh/id_rsa

- tail ~/.ssh/id_rsa.pub

## Push Commands 
git push -u origin master

## Aliacing commands
git config --global alias.unstage 'restore --staged --'
git config --global alias.last 'log -p -1'

## Checkout commands

- git checkout -b develop 

## Branch Commands
### To check the existing branches
- git branch 

### To delete a remote brach
- git push remote--delete branchname  

### To switch to a particular branch
- git checkout bhranchname  To switch to a particular branch

### To create a new branch
- git branch newbranchname  

### To merge a branch
- git merge branchname  

