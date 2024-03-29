# Git Task

## Table Of Contents
- [Version control](#version-control)
- [Difference between Git and GitHub](#difference-between-git-and-github)
- [Git & GitHub Alternatives](#git--github-alternatives)
- [Difference Between Git Fetch & Git Pull](#difference-between-git-fetch--git-pull)
- [Git Rebase](#git-rebase)
  - [Git Rebase Command](#git-rebase-command)
- [Git Cherry-pick](#git-cherry-pick)
  - [Git Cherry-pick Command](#git-cherry-pick-command)

## Version Control
Version control is a process of creating different instances of a project in order to track changes in the project. Version control also allows us to rollback to a previous version in case of any issues with the project. With version control, different people can contribute to the project at once.

## Difference Between Git and GitHub.
__Git__ is a Version Control System. It is used for tracking, collaboration and also to revert to previous changes. It is used to take snapshots of our code.

__GitHub__ on the other hand is a remote repository used to house our code source files, also keeping track of the different versions and branches. GitHub is also used to host our projects.

While both are different, and can work independently, they mostly are used side by side, because as a unit, its a powerful tool in the hands of a developper.

## Git & GitHub Alternatives
__Git Alternatives:__ Mecurial, Perforce, BitBucket <br>
__GitHub Alternatives:__ GitLab, GitKraken, Azure Devops


## Difference Between Git Fetch & Git Pull
__Git Fetch:__ This is a git command that is used for getting the updates from the remote to local. This command is used when you don't want to integrate the changes immediately.

__Git Pull:__ Git Pull combines two commands into one command, which is the `git fetch` and the `git merge`. It first fetches the changes and then automatically merges them to the codebase in the local. 

While they're similar, the former is used mostly when we want to review a new update before merging with what we have, while the latter is used to automatically retrieve and merge. 

## Git Rebase 
Git rebase is basically a command that combines a sequence of commits to a new base. It is basically taking your changes in another branch and stacking it on top of the .changes already made to the other branch in a logical order. It makes the codebase cleaner and easier to find where an issue is coming from. 

#### Git Rebase Command
```
git rebase <base>
```

## Git Cherry-pick
Git cherry-pick is a useful command that enbles commands to be picked and appended to the current working branch/HEAD. Assuming we have branch A, which is the main, and branch B, which can be a feature branch, we can cherry-pick a particular commit from branch B and append it to branch A.

Git cherry-pick is also similar to Git rebase, with the difference being that rebase appends every commit in the selected branch and appends it to the current branch, while cherry-pick picks out particular commits from the branch and appends it to the current branch

#### Git Cherry-pick Command

```
git cherry-pick <commit-hash>
```

or

```
git cherry-pick <branch-name>^
```
The caret selects the last commit in the particular branch