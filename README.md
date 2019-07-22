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
8. Check out the commit history of your merge-main branch.
9. Go back into your merge-main branch.
10. Create a new branch named merge-feature-4.
3. Create some commits on your merge-feature-3 and merge-feature-4 branch.
11. Push your merge-feature-3 and merge-feature-4 branch into your remote repo.
12. Create a pull request to merge the merge-main and merge-feature-3 and merge-feature-4 branch.
13. Review and merge your changes.
14. Pull the changes on merge-main.
15. Check out the commit history of your merge-main branch.

_Do you notice the difference in the commit history when you're working with a single branch at a time and working
with multiple branch at the same time?_

## Activity Three: Using Rebase

How do we keep an organize history while working with multiple branches? The answer is we rebase!

We're going to follow similar steps that we took during activity two except we will rebase our branch before merging it into our main branch 

1. Go into your rebase-main branch.
2. This time create two new branches: rebase-feature-1 and rebase-feature-2.
3. Create some commits on your rebase-feature-1 branch.
_Your branch is currently based on the most recent commit of master so rebasing will not do anything._
4. Push your rebase-feature-1 branch into your remote repo.
5. Create a pull request to merge the rebase-main and rebase-feature-1 branch.
6. Review and merge your changes.
7. Pull the changes on rebase-main.
8. Check out the commit history of your rebase-main branch.
_So far everything should look very similar to activity 2, but that is about to change._
9. Go back into your rebase-main branch.
10. Create a new branch named rebase-feature-3.
11. Create some commits on your rebase-feature-2 and rebase-feature-3 branch.
12. Rebase your rebase-feature-2 branch onto rebase-main.
13. Push your rebase-feature-2 branch into your remote repo.
14. Create a pull request to merge the rebase-main and rebase-feature-2.
15. Review and merge your changes.
16. Pull the changes on rebase-main.
17. Before we rebase rebase-feature-3, check out the commit history of rebase-feature-3.
18. Rebase your rebase-feature-3 branch onto master.
_Check the commit history or rebase-feature-3, does it look different?_
19. Push your rebase-feature-3 branch into your remote repo.
20. Create a pull request to merge the rebase-main and rebase-feature-3.
21. Review and merge your changes.
22. Pull the changes on rebase-main.
23. Check out the commit history of your rebase-main branch.

_Compare the history of commits on merge-main vs. rebase-main, what do you notice?_

## Git Command Cheat Sheet

|Command|Results|
|-------|-------|
|```git branch [branch name]```|Creates a new branch.|
|```git checkout [branch name]```|Switches to the branch.|
|```git checkout -b [branch name]```|Creates a new branch and switches to it.|
|```git add .```|Adds all changes in the repo to the staging area.|
|```git commit -m [log message]```|Commits all the changes in the staging area.|
|```git pull [branch name]```|Updates your local repo based on your remote repo.|
|```git push -u origin [branch name]```|Pushes your local branch for the first time into the remote repo.|
|```git rebase master [branch name]```| Moves the starting point of your branch to the most recent commit on master.|
|```git log --graph --oneline```|Visually displays your commit history|
