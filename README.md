# Git Guide
## Table of Contents
- [Credentials](#credentials)
  - [Set Credentials](#set-credentials)
  - [Remove Credentials](#remove-credentials)
- [Initialize Repository](#initialize-repository)
- [Stage](#stage)
  - [Add All (Root)](#add-all-root)
  - [Add All (Current Directory)](#add-all-current-directory)
  - [Add File](#add-file)
  - [Unstage All (Current Directory)](#unstage-all-current-directory)
  - [Unstage File](#unstage-file)
  - [Add Everything](#add-everything)
  - [Unstage All](#unstage-all)
  - [Unstage File](#unstage-file)
- [Remote Repository](#remote-repository)
  - [Add URL](#add-url)
  - [Update/Set URL](#update-set-url)
  - [Pull](#pull)
- [Branching](#branching)
  - [Create branch](#create-branch)
  - [Rename branch](#rename-branch)
  - [Switch branch](#switch-branch)
  - [Merge to current branch](#merge-to-current-branch)
  - [Delete branch after merging](#delete-branch-after-merging)
  - [Delete branch before merging](#delete-branch-before-merging)
  - [Delete remote branch](#delete-remote-branch)
---
## Credentials
### Set Credentials
```
git config --global user.name "username"
```
```
git config --global user.email "email"
```
### Remove Credentials
```
git config --global --unset user.name
```
```
git config --global --unset user.email
```
## Initiallize Repository
```
git init
```
## Stage
### Add All (Root)
```
git add -A
```
### Add All (Current Directory)
```
git add .
```
### Add File
```
git add <filename>
```
### Unstage All (Current Directory)
```
git reset .
```
### Unstage File
```
git reset <filename>
```
## Remote Repository
### Add URL
```
git remote add origin <url>
```
### Update/Set URL
```
git remote set-url origin <url>
```
### Pull
```
git pull origin <branch>
```
## Branching
### Create branch
```
git branch <branch_name>
```
### Rename branch
```
git branch -M <branch_new_name>
```
### Switch branch
```
git switch <another_branch>
```
### Merge to current branch
```
git merge wip
```
### Delete branch after merging
```
git branch -d <merged_branch>
```
### Delete branch before merging
```
git branch -D <unmerged_branch>
```
### Delete remote branch
```
git push origin --delete <branch_to_delete>
```
---
## Stage
```
git add .
```
```
git reset .
```
## Status
```
git status
```
## Commit
```
git commit -m "first commit"
```
## Reset
```
git reset --hard <hash>
```
## Rebase
```
git rebase -i <hash>
```
## Log
```
git log
```
## Push
```
git push origin main
```
## Force Push
```
git push origin main --force
```
## Remote Delete Branch
```
git push origin --delete wip
```


<!--
chore: Maintenance tasks (e.g., build tools, dependencies)
feat: A new feature
fix: A bug fix
docs: Documentation changes
style: Code formatting (no logic change)
refactor: Code restructuring without functionality changes
perf: Performance improvements
test: Adding or updating tests
ci: CI/CD-related changes
revert: Reverting a previous commit

fix: fix foo to enable bar
This fixes the broken behavior of the component by doing xyz. 
BREAKING CHANGE
Before this fix foo wasn't enabled at all, behavior changes from <old> to <new>
Closes D2IQ-12345 
-->


<!-- ## Other Commands
git rm --cached todo.txt
git filter-branch --force --index-filter \
"git rm --cached --ignore-unmatch todo.txt" \
--prune-empty --tag-name-filter cat -- --all -->

