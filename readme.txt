 Git Cheat Sheet

First `hit`a new repository to work with:
...
$ git init REPO_NAME
$ cd REPO_NAME
...

*NOTE*
Directories are not tracked, just add a `.keep` file

To ignore files add them to `.gitignore`:
...
log/*.log
...

To just add parts to the ind we can use `git add -p`(`-p`as in "patch").

## Disaster Recovery

In case of delete commits use `git reflog`and `git cherry-pick` to recover those commits: 
...
$ git cherry-pick LOST_COMMIT_SHA1
...

**NOTE** Will be cleaned up once `git gc`ran

