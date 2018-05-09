# git-quick-reference

#### refresh list of remote branches at `origin`

`git remote update origin --prune`

#### delete a branch at remote `origin`

`git push -d origin some-branch`

#### delete a local branch

`git branch -d some-branch`

#### show the complete history of a file

`git log --follow -p -- filename`

Reference: https://stackoverflow.com/a/5493663/5360439

#### show who last modified each line of a file

`git blame -L 40,60 filename`

#### setup upstream remote for a fork

`git remote add upstream https://github.com/owner/repo.git`

#### syncing a fork with upstream branch

```bash
git fetch upstream develop
git checkout develop
git merge upstream/develop

```
Reference: https://help.github.com/articles/syncing-a-fork/

#### find the parent branch of a git branch

Reference: https://stackoverflow.com/questions/3161204/find-the-parent-branch-of-a-git-branch/3162929#3162929

#### set remote url

`git remote set-url origin https://github.com/user/repo.git`

#### rename a git branch

to rename current branch,

`git branch -m newname`

else,

`git branch -m oldname newname`

It will add a new branch to the remote when it's pushed, but the old branch won't be deleted.

#### stage files with regular expression

`git add src/*.cpp`
