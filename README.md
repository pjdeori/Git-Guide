## Table of Contents
- [Information](#information)
  - [Set Credentials](#set-credentials)
  - [Remove Credentials](#remove-credentials)
  - [Initialize Repository](#initiallize-repository)
  - [Commit Log](#commit-log)
- [Stage](#stage)
  - [Status](#status)
  - [Add All (Root)](#add-all-root)
  - [Add All (Current Directory)](#add-all-current-directory)
  - [Add File](#add-file)
  - [Unstage All (Current Directory)](#unstage-all-current-directory)
  - [Unstage File](#unstage-file)
- [Remote Repository](#remote-repository)
  - [Add URL](#add-url)
  - [Update URL](#update-url)
  - [Pull](#pull)
  - [Commit](#commit)
  - [Push](#push)
  - [Remote Delete Branch](#remote-delete-branch)
- [Branching](#branching)
  - [Create branch](#create-branch)
  - [Rename branch](#rename-branch)
  - [Switch branch](#switch-branch)
  - [Merge to current branch](#merge-to-current-branch)
  - [Delete branch after merging](#delete-branch-after-merging)
  - [Delete branch before merging](#delete-branch-before-merging)
  - [Delete remote branch](#delete-remote-branch)

---
## Information
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
### Initiallize Repository
```
git init
```
### Commit Log
```
git log
```
## Stage
### Status
```
git status
```
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
### Update URL
```
git remote set-url origin <url>
```
### Pull
```
git pull origin <branch>
```
### Commit
```
git commit -m "commit message"
```
### Push
```
git push origin <branch>
```
### Remote Delete Branch
```
git push origin --delete <branch>
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