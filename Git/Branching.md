# Branching

## What is a Branch?

A branch is an independent line of development.

Allows developers to work without affecting the main codebase.

---

## Why Branching?

* Feature development
* Bug fixes
* Experimentation
* Release management

---

## Default Branch

Traditionally:

main

or

master

---

## View Branches

git branch

---

## Create Branch

git branch feature-login

---

## Switch Branch

git checkout feature-login

Modern Method:

git switch feature-login

---

## Create and Switch

git checkout -b feature-login

OR

git switch -c feature-login

---

## Branch Workflow

main
│
├── feature-login
│
├── feature-payment
│
└── feature-api

---

## Merge Branch

git checkout main

git merge feature-login

---

## Delete Branch

git branch -d feature-login

Force Delete:

git branch -D feature-login

---

## Remote Branches

View:

git branch -r

Fetch:

git fetch

Pull:

git pull

---

## Best Practices

* Use descriptive names
* Keep branches small
* Delete merged branches
* Create Pull Requests

---

## Naming Convention

feature/login

feature/payment

bugfix/authentication

hotfix/api

release/v1.0

---

## Interview Questions

Q: Why use branches?

A: To isolate development work from production code.

Q: Difference between merge and rebase?

A: Merge preserves history; rebase rewrites history.

Q: What is a feature branch?

A: Branch created for implementing a specific feature.
