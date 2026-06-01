# Merge Strategies

## Overview

Git provides multiple ways to combine branches.

---

## Fast Forward Merge

Occurs when no new commits exist on target branch.

Example:

main

A → B

feature

A → B → C

Merge:

A → B → C

Command:

git merge feature

---

## Three-Way Merge

When both branches have commits.

Example:

main

A → B → D

feature

A → B → C

Merge Result:

A → B → C → D → M

---

## Squash Merge

Combines all commits into one commit.

Command:

git merge --squash feature

Benefits:

* Clean history
* Easier tracking

---

## Rebase

Moves commits onto another base branch.

Command:

git rebase main

Benefits:

* Linear history
* Cleaner logs

---

## Merge Conflict

Occurs when two branches modify same file section.

Example:

<<<<<<< HEAD
Version A
=========

Version B

> > > > > > > feature

Resolve manually.

---

## Conflict Resolution Workflow

1. Open File
2. Resolve Conflict
3. Save File
4. Add File

git add .

5. Commit

git commit

---

## Cherry Pick

Apply specific commit.

git cherry-pick COMMIT_ID

---

## Best Practices

* Pull latest changes
* Keep commits small
* Rebase feature branches
* Resolve conflicts early

---

## Interview Questions

Q: What is rebase?

A: Rebase moves commits to a new base commit.

Q: What is squash merge?

A: Combines multiple commits into one commit.

Q: What causes merge conflicts?

A: Modifications to the same lines in a file.
