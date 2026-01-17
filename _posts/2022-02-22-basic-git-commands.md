---
title: Basic git commands
description: >-
  This guide includes the basic git commands which are useful for all the GitHub users. 
author: swapnilmali101
date: 2022-02-22 12:00:00 +0530
categories: [DevOps, Cheatsheets]
tags: [git, github, bash, terminal]
pin: true
media_subpath: '/assets/img/'
image: 
  path: /Basic-git-commands.png
  alt: Basic-git-commands
---

🔗 : If you want the pdf version then [Download the PDF]({% link assets/files/Basic git commands created by swapnil mali.pdf %})

◨◧ How to initialize git for directory as local git repository?
```
~$ git init
~$ git init <repo-name>
```
> 👉: repo-name = specify directory for local git repository

◨◧ How to configure git to user ?
```
~$ git config --global user.name <user-name>
~$ git config --global user.email <user-email>

~$ git config --local user.name <user-name>
~$ git config --local user.email <user-email>
```
> 👉: flag {global} for all repositories

> 👉: flag {local} for specific repository

> 👉: user-name = specify user name

> 👉: user-email = specify user email address

◨◧ How to show tracking of files ?
```
~$ git status
```
◨◧ How to clone git repository from remote server?
```
~$ git clone <repo-url>
```
> 👉: repo-url = remote repository url

◨◧ How to staged changes in files (i.e. ready to commit) ?
```
~$ git add <file-name>
~$ git add .
```
> 👉: file-name = specify file name or use "." to specify all files

◨◧ How to commit staged changes ?
```
~$ git -commit -m "message"
```
> 👉: message = use present tenses recommended

◨◧ How to create main branch ?
```
~$ git branch -M main
~$ git remote add origin <repo-url>
```
> 👉: repo-url = specify repository url to create main branch

◨◧ How to push commits to main branch ?
```
~$ git push -u origin main
```
◨◧ How to create new branch ?
```
~$ git branch -b <branch-name>
```
> 👉: branch-name = specify name of branch

◨◧ How to push commits to specific branch ?
```
~$ git push -u origin <branch-name>
```
◨◧ How to change branch (i.e. hopping between branches) ?
```
~$ git checkout <branch-name>
```
◨◧ How to check all git commits which are not in local branch ?
```
~$ git fetch origin
```
◨◧ How to pull all changes to local branch ?
```
~$ git pull origin <branch-name>
```
◨◧ How to initialize and checkout branch ?
```
~$ git checkout -b <branch-name>
```
◨◧ How to merge another branch into current branch ?
```
~$ git merge <branch-name>
```
◨◧ How to show all conflicts between branches before merging them ?
```
~$ git diff
```
◨◧ How to mark specific commits ?
```
~$ git tag <commit-tag>
```
> 👉: commit-tag = specify tag to recognize commit

◨◧ How to undo changes ?
```
~$ git revert
```
◨◧ How to reset branch to last commited state ?
```
~$ git reset --hard HEAD
```
◨◧ How to remove file from current repository ?
```
~$ git rm <file-name>
```
◨◧ How to keep commit to side tray for further use ?
```
~$ git stash
```
◨◧ How to use side tray commit into current branch?
```
~$ git stash pop
```
