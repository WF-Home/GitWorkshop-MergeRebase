# Git Workshop || Merge VS. Rebase

### Setup

* Fork and clone this repo.
* Create a branch from master named merge-main and rebase-main.
```
git branch merge-main
```
```
git branch rebase-main
```
* Push the new branches into the remote repo.
```
git checkout merge-main
git push -u origin merge-main
```
```
git checkout rebase-main
git push -u origin rebase-main
```

## Activity One: Merging a Single Branch

1. Go into your merge-main branch.
2. Create a new branch named merge-feature-1.
3. Create some commits on your merge-feature-1 branch.
4. Push your merge-feature-1 branch into your remote repo
5. Create a pull request to merge the merge-main and merge-feature-1 branch.
6. Review and merge your changes.
7. Update your local repo.
8. Check out your commit history.

## Activity Two: Working with Multiple Branches

## Activity Three: Using Rebase

## Git Command Cheat Sheet

|Command|Results|
|-------|-------|
|```git branch [branch name]```|Creates a new branch.|
|```git checkout [branch name]```|Switches to the branch.|
|```git checkout -b [branch name]```|Creates a new branch and switches to it.|
|```git pull [branch name]```|Updates your local repo based on your remote repo.|
|```git push -u origin [branch name]```|Pushes your local branch for the first time into the remote repo.| 
|```git log --graph --oneline```|Visually displays your commit history|
