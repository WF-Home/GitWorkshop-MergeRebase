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
Before we get started, check out the current history of commits. 
```
git log --graph --oneline
```
This is the ideal history we want to achieve.

## Activity One: Merging a Single Branch

1. Go into your merge-main branch.
2. Create a new branch named merge-feature-1.
3. Create some commits on your merge-feature-1 branch.
4. Push your merge-feature-1 branch into your remote repo.
5. Create a pull request to merge the merge-main and merge-feature-1 branch.
6. Review and merge your changes.
7. Pull the changes on merge-main.
8. Check out your commit history.

## Activity Two: Working with Multiple Branches

1. Go into your merge-main branch.
2. This time create two new branches: merge-feature-2 and merge-feature-3.
3. Create some commits on your merge-feature-2 branch.
4. Push your merge-feature-2 branch into your remote repo.
5. Create a pull request to merge the merge-main and merge-feature-2 branch.
6. Review and merge your changes.
7. Pull the changes on merge-main.
8. Check out your commit history.
9. Go back into your merge-main branch.
10. Create a new branch named merge-feature-4.
3. Create some commits on your merge-feature-3 and merge-feature-4 branch.
11. Push your merge-feature-3 and merge-feature-4 branch into your remote repo.
12. Create a pull request to merge the merge-main and merge-feature-3 and merge-feature-4 branch.
13. Review and merge your changes.
14. Pull the changes on merge-main.
15. Check out your commit history.

Do you notice the difference in the commit history when you're working with a single branch at a time and working
with multiple cranch at the same time?


## Activity Three: Using Rebase

## Git Command Cheat Sheet

|Command|Results|
|-------|-------|
|```git branch [branch name]```|Creates a new branch.|
|```git checkout [branch name]```|Switches to the branch.|
|```git checkout -b [branch name]```|Creates a new branch and switches to it.|
|```git pull [branch name]```|Updates your local repo based on your remote repo.|
|```git push -u origin [branch name]```|Pushes your local branch for the first time into the remote repo.|
|```git rebase master [branch name]```| Moves the starting point of your branch to the most recent commit on master.|
|```git log --graph --oneline```|Visually displays your commit history|
