# git-quick-reference

####1. refresh list of remote branches at `origin`

`git remote update origin --prune`

####2. delete a branch at remote `origin`

`git push -d origin some-branch`

####3. delete a local branch

`git branch -d some-branch`

####4. show the complete history of a file

`git log --follow -p -- filename`

Reference: https://stackoverflow.com/a/5493663/5360439

####5. show who last modified each line of a file

`git blame -L 40,60 filename`

####6. setup upstream remote for a fork

`git remote add upstream https://github.com/owner/repo.git`

####7. syncing a fork with upstream branch

```bash
git fetch upstream develop
git checkout develop
git merge upstream/develop

```
Reference: https://help.github.com/articles/syncing-a-fork/

####8. find the parent branch of a git branch

Reference: https://stackoverflow.com/questions/3161204/find-the-parent-branch-of-a-git-branch/3162929#3162929

####9. set remote url

`git remote set-url origin https://github.com/user/repo.git`
