
git init
initialize an existing directory as a Git repository

git status
show modified files in working directory, staged for your next commit


Clone fresh project

git clone -b master https://github.com/sadanandchavan/sbdb.git

Branch List
$ git branch

Delete Branch
$ git branch -d <branch_name>

Create Branch
git checkout -b <branch_name>

Pull from dev
$ git pull

Switch
$ git switch dev

Pull from branch
$ git pull origin <branch_name>

Add file for commit
$ git add src/java/com/ABCD.java


unstage a file while retaining the changes in working directory
git reset [file]

diff of what is changed but not staged
git diff

diff of what is staged but not yet commited
git diff --staged
	

List of files for push
$ git diff --stat --cached origin/dev

hat is about to be committed 
git diff --cached

Push branch
git push -u origin <branch_name>

chnaged file name-only
git diff --name-only SHA1 SHA2


Changed files between the last commit and the one before it
git show --name-only


git branch

list your branches. a * will appear next to the currently active branch

git branch [branch-name]
create a new branch at the current commit

git checkout
switch to another branch and check it out into your working directory

git merge [branch]
merge the specified branch’s history into the current one

git log
show all commits in the current branch’s history


git log
show the commit history for the currently active branch
git log branchB..branchA
show the commits on branchA that are not on branchB
git log --follow [file]
show the commits that changed file, even across renames
git diff branchB...branchA
show the diff of what is in branchA that is not in branchB
git show [SHA]
show any object in Git in human-readable format

git remote add [alias] [url]
add a git URL as an alias
git fetch [alias]
fetch down all the branches from that Git remote
git merge [alias]/[branch]
merge a remote branch into your current branch to bring it up to date
git push [alias] [branch]
Transmit local branch commits to the remote repository branch
git pull
fetch and merge any commits from the tracking remote branch

git rm [file]
delete the file from project and stage the removal for commit
git mv [existing-path] [new-path]
change an existing file path and stage the move
git log --stat -M
show all commit logs with indication of any paths that moved

git rebase [branch]
apply any commits of current branch ahead of specified one
git reset --hard [commit]
clear staging area, rewrite working tree from specified commit


git stash
Save modified and staged changes
git stash list
list stack-order of stashed file changes
git stash pop
write working from top of stash stack
git stash drop
discard the changes from top of stash stack



Merge Conflict

vi editor

Press i (i for insert)
Write your merge message
Press esc (escape)
Write :wq (write & quit)
Then press enter


