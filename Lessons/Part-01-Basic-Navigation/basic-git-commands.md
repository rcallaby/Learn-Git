## Basic Git Commands


To clone a repository to your local.

```sh
git clone [URL]
```

Initialize an existing directory as a Git repository.
```sh
git init
```
To stage a file so that it can be committed.
```sh
git add <file name\> 
```
To commit the added file along with a message.
```sh
git commit -m “message”
```
To push the changes made to the file locally to the GitHub repository.
```sh
git push origin <branch name\>
```
Unstaged a file while retaining the changes in the working directory.
```sh
git reset <file name\>
```
Difference of what is changed but not staged.
```sh
git diff
```
List your branches. * Indicates the currently active branch.
```sh
git branch
```
Create a new branch at the current commit.
```sh
git branch <branch-name>
```
Switch to another branch and check it out in your working directory.
```sh
git checkout
```
Merge the specified branch’s history into the current one.
```sh
git merge <branch\>
```
Show all commits in the current branch’s history
```sh
git log
```
Delete the file from the project and stage the removal for commit.
```sh
git rm <file\>
```
Fetch down all the branches from that Git remote
```sh
git fetch [alias]
```
Merge a remote branch into your current branch to bring it up to date
```sh
git merge [alias]/[branch]
```
Fetch and merge any commits from the tracking remote branch
```sh
git pull
```
Combining your local unpublished changes with the latest published changes on your remote
```sh
git pull –rebase
```
Save modified and staged changes
```sh
git stash
```
Write working from the top of the stash stack
```sh
git stash pop
```
Discard the changes from the top of the stash stack
```sh
git stash drop
```
