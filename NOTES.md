# GIT-COMMANDS

### Deletions Commands
- deleting a .git folder from a repo
rm -rf .git 

### To add all changes to the staging area
git add --a 

### Git ignore commands
- touch .gitignore
- error.log
- *.log
- dir/
- /dir/ to track only outer dir it'll skip the inner one
- git by defaultly ignores the blank directories

### comarison commands

- git diff will compare the working  directory and staging area

- git diff --staged

### commit cmmands
- git commit -a -m "your comment"
- This will commit all the tracked files untracked file needs to be added specially
- git commit --amend  ---> to make changes in the commit

### Basic Commands 

- git rm file.txt --> remove
- git mv file.txt file_01.txt ---> to rename files

-  Untracking files
git rm --cached db.accdb 

### git log commands

- git log -p --> to check commits + files deleted
- git log -3 --->or -2 to check specific commits
- git log -p -1 ---> to check individual commits
- git log --stat ---> to check more specif on commits
- git log --pretty=oneline
- git log --pretty=short
- git log --pretty=full
- git log --since=2.days --> filter according to time
- git log --since=2.year/months/years
- git log pretty=format:"%h --%an or ae"

git commit --amend  ---> to make changes in the commit
git restore --staged ---> To remove any file from staging area
git checkout --filename.txt --> To checkout to the previous commit
git checkout -f  ----> All the changes to vanish and move to the previous commit
as a clean tree

git remote

git remote add origin git@github.com:rudrakshkarpe/repositoryname.git

git remote -v

ssh-keygen -t rsa 4096 -C "rudraksh.karpe@gmail.com"

 eval $(ssh-agent -s)

ssh-add ~/.ssh/id_rsa

tail ~/.ssh/id_rsa.pub

git push -u origin master

git config --global alias.unstage 'restore --staged --'
git config --global alias.last 'log -p -1'

git checkout -b develop --> to create a new branch and switch to it

git branch to check the existing branches
git push remote--delete branchname ---> to delete a remote brach
git checkout bhranchname ---> To switch to a particular branch
git branch newbranchname ----> To create a new branch
 git merge branchname ---> To merge a particular banch

