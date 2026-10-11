# Proof of Work — DevOps Git Challenge

## Repository
https://github.com/sudais45803/devops-git-challenge

## Student
Name: Sudais Maqsood
Email: 45803@students.riphah.edu.pk

## Branches Created
- main
- development
- staging

## Commands Executed
- git config --global user.name / user.email
- git clone https://github.com/sudais45803/devops-git-challenge.git
- git add . && git commit -m "feat: initial commit with deploy script"
- git checkout -b development
- git stash / git stash pop
- git checkout -b staging
- git merge staging (conflict resolved)
- git push origin development
- git push origin staging
- git pull origin main

## Pull Request
- PR #1: Merge development into main — MERGED

## Screenshots
All screenshots are attached separately with the submission.

## Commit History

[
*   edcc1c0 (HEAD -> main, origin/main) Merge pull request #1 from sudais45803/development
|\  
| *   e2fb6f5 (origin/development, development) fix: resolved merge conflict
| |\  
| | * fc6f112 (origin/staging, staging) fix: staging label
| |/  
|/|   
| * 9c77956 feat: updated script with staging env
|/  
* b8d391d feat: initial commit with deploy script
]
## Reflection Questions

### Q1: Difference between Git (local tracking) and GitHub (cloud platform)
Git is a distributed version control system installed locally that tracks file changes, creates commits, and manages branches without needing the internet. GitHub is a cloud-based hosting platform built on top of Git that stores remote repositories and enables collaboration via pull requests, issues, and code reviews. Git works entirely offline, while GitHub requires network access and adds social and collaboration features. In short, Git is the tool; GitHub is the service that hosts Git repositories.

### Q2: Explain the 3 architecture stages: Working Directory, Staging Area, Local Repository
The Working Directory is the local folder where files are edited; changes here are untracked or modified. The Staging Area (Index) is a holding zone where files are prepared with `git add` before committing. The Local Repository is the `.git` database on the machine that permanently stores committed snapshots. The flow is: Working Directory → `git add` → Staging Area → `git commit` → Local Repository → `git push` → Remote.

### Q3: Difference between `git stash pop` and `git stash apply`
Both commands restore stashed changes to the working directory. `git stash pop` restores the changes and removes the stash entry from the stash list. `git stash apply` restores the changes but keeps the stash in the list for reuse. Use `apply` when you want to reapply the same stash to multiple branches; use `pop` for a one-time restore.

### Q4: Difference between `git fetch` and `git pull`
`git fetch` downloads new commits, branches, and tags from the remote into the local repository without modifying the working directory or current branch. `git pull` is essentially `git fetch` followed by `git merge` (or rebase), so it downloads and integrates changes into the current branch. `fetch` is safer for reviewing changes first; `pull` is faster when you trust the remote updates.
