# Git Commands Cheat Sheet

## Configuration

git config --global user.name "John"

git config --global user.email "[john@gmail.com](mailto:john@gmail.com)"

git config --list

---

## Repository

git init

git clone URL

git status

---

## Staging

git add file.txt

git add .

git reset file.txt

---

## Commit

git commit -m "message"

git commit --amend

---

## Branching

git branch

git branch feature-login

git switch feature-login

git switch -c feature-login

git branch -d feature-login

---

## Merging

git merge feature-login

git merge --squash feature-login

---

## Rebase

git rebase main

git rebase --continue

git rebase --abort

---

## Remote Repository

git remote -v

git remote add origin URL

---

## Push

git push origin main

git push -u origin main

---

## Pull

git pull origin main

---

## Fetch

git fetch

---

## Logs

git log

git log --oneline

git log --graph

git log --decorate

---

## Undo Changes

git restore file.txt

git checkout -- file.txt

git reset HEAD~1

---

## Stash

git stash

git stash list

git stash pop

---

## Tags

git tag

git tag v1.0

git push origin v1.0

---

## Compare Changes

git diff

git diff --staged

git show

---

## Cherry Pick

git cherry-pick COMMIT_ID

---

## Useful Commands

git branch -a

git remote -v

git reflog

git clean -fd

git blame file.txt

git shortlog

git show

---

## Top 20 Git Commands for DevOps

1. git clone
2. git status
3. git add
4. git commit
5. git push
6. git pull
7. git fetch
8. git branch
9. git switch
10. git checkout
11. git merge
12. git rebase
13. git stash
14. git log
15. git diff
16. git tag
17. git remote
18. git reset
19. git restore
20. git cherry-pick

---

## DevOps Interview Focus

Master:

* Branching
* Merge vs Rebase
* Pull Requests
* Stash
* Cherry Pick
* Git Reset
* Git Reflog
* Merge Conflicts
* GitHub Workflow
* GitHub Actions
