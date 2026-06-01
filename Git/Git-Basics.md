# Git Basics

## What is Git?

Git is a distributed version control system used to track changes in source code and collaborate with other developers.

Created by Linus Torvalds in 2005.

## Why Git?

* Tracks code changes
* Maintains version history
* Supports collaboration
* Enables rollback to previous versions
* Essential for DevOps CI/CD workflows

---

## Version Control Systems

### Local VCS

Stores versions locally.

### Centralized VCS

Examples:

* SVN
* CVS

### Distributed VCS

Examples:

* Git
* Mercurial

Git is Distributed.

---

## Git Architecture

Working Directory
↓
Staging Area
↓
Local Repository
↓
Remote Repository

### Working Directory

Current files being edited.

### Staging Area

Files prepared for commit.

### Repository

Stores commit history.

---

## Git Workflow

1. Create File
2. Stage File
3. Commit Changes
4. Push to GitHub

Example:

git add .

git commit -m "Initial Commit"

git push origin main

---

## Git Installation

Ubuntu:

sudo apt update
sudo apt install git

Verify:

git --version

---

## Configure Git

Set Username:

git config --global user.name "John Doe"

Set Email:

git config --global user.email "[john@gmail.com](mailto:john@gmail.com)"

View Configuration:

git config --list

---

## Create Repository

git init

Check Status:

git status

---

## First Commit

touch app.py

git add app.py

git commit -m "Added application"

---

## Git Objects

### Blob

Stores file content.

### Tree

Stores directory structure.

### Commit

Stores snapshot.

---

## Git States

* Modified
* Staged
* Committed

---

## Common Workflow

git pull

git add .

git commit -m "Changes"

git push

---

## Interview Questions

Q: What is Git?

A: Git is a distributed version control system used to manage source code changes.

Q: Difference between Git and GitHub?

A: Git is a version control tool; GitHub is a cloud platform for Git repositories.

Q: What is a commit?

A: A snapshot of changes stored in Git history.

---

## Hands-On Lab

1. Install Git
2. Configure Git
3. Create Repository
4. Create File
5. Commit Changes
6. Push to GitHub
