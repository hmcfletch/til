# Git

TIL's about the Git

### Scratch

* which local branchs can be pruned
    - `git checkout master`
    - `git branch --merged`
    - `git branch -d old-merged-feature`
* undo last commit 
    - `git reset --soft HEAD~1`
* [add upstream](https://help.github.com/articles/configuring-a-remote-for-a-fork/)
    - `git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git`
* list remote branches
    - `git branch -r`
