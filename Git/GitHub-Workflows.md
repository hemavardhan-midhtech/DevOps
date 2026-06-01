# GitHub Workflows

## What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories.

---

## Typical Workflow

Developer
↓
Feature Branch
↓
Commit
↓
Push
↓
Pull Request
↓
Code Review
↓
Merge
↓
Deploy

---

## Clone Repository

git clone REPOSITORY_URL

---

## Add Remote Repository

git remote add origin URL

Verify:

git remote -v

---

## Push Code

git push origin main

---

## Pull Code

git pull origin main

---

## Fetch Changes

git fetch

---

## Pull Request Workflow

1. Create Branch
2. Commit Changes
3. Push Branch
4. Create Pull Request
5. Review
6. Merge
7. Delete Branch

---

## Fork Workflow

Fork Repository
↓
Clone Fork
↓
Create Branch
↓
Commit
↓
Push
↓
Pull Request

---

## GitHub Actions

GitHub's CI/CD Platform.

Example:

Build
Test
Deploy

Workflow File:

.github/workflows/main.yml

---

## Protected Branches

Prevent direct modifications.

Common Rules:

* Pull Request Required
* Reviews Required
* Status Checks Required

---

## Repository Best Practices

* Meaningful README
* Branch Protection
* Pull Requests
* CI/CD Pipelines
* Documentation

---

## Interview Questions

Q: What is a Pull Request?

A: A request to merge code changes into another branch.

Q: Difference between Pull and Fetch?

A: Fetch downloads changes; Pull downloads and merges changes.

Q: What is GitHub Actions?

A: GitHub's native CI/CD automation platform.
