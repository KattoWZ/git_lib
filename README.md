# 🐙 Git Cheat Sheet for Project Management

This cheat sheet is a handy guide for managing branches, commits, merges, and other common Git tasks while working on your project.

---

## 📦 Repository Initialization

```bash
git init
```
Initialize a new Git repository in the current directory.

---

## 📥 Cloning a Repository

```bash
git clone <repo_url>
```
Clone a remote repository to your local machine.

---

## 🔍 Status Check

```bash
git status
```
Show the status of changes in your working directory.

---

## ➕ Staging Files

```bash
git add <filename>
git add .
```
Add specific files or all changes to the staging area.

---

## 📝 Committing Changes

```bash
git commit -m "Your descriptive commit message"
```
Commit staged changes with a message.

---

## 📂 Committing Specific Files

```bash
git add fileA.py
git commit -m "Update fileA.py for feature X"
```
Add and commit a specific file independently.

---

## 🚫 Removing Files from Git Tracking

```bash
git rm --cached <file_or_folder>
```
Remove a file or folder from the repository (but keep it locally).

---

## 📄 `.gitignore` Example

```gitignore
venv/
__pycache__/
log/
```
Ignore virtual environments, cache folders, and logs.

---

## ⬇️ Pulling Updates

```bash
git pull
```
Fetch and merge updates from the remote repository.

---

## ⬆️ Pushing Changes

```bash
git push
```
Push your committed changes to the remote repository.

---

## 🌿 Branching

```bash
git branch dev
git checkout dev
```
Create and switch to a development branch.

---

## 🔀 Merging Branches

```bash
git checkout main
git merge --no-ff dev -m "Merge dev into main"
```
Merge changes from `dev` to `main` with a commit message (preserving commit history).

---

## 🧾 Viewing Commits

```bash
git log
```
View the history of commits.

---

## 🧹 Undo a Commit (Soft Reset)

```bash
git reset --soft HEAD~1
```
Undo the last commit but keep the changes staged.

---

## 📎 Stashing Work

```bash
git stash
git stash pop
```
Temporarily save and restore uncommitted changes.

---
# 🏷️ Git Tagging System Guide

Git tags are used to mark specific points in a repository’s history as important — usually for **releases**, **version control**, or **milestone tracking**.

## 📌 Tagging Basics

### 🔹 Create a Lightweight Tag
```bash
git tag <tag_name>
git push origin <tag_name>
```
Create and push a version tag to the remote repo.

### Delete a tag
```bash
git tag -d <tag_name>
git fetch --prune-tags
```
The `fetch --prune-tags` is to check if the tag is already deleted on the remote or not
---

## 🔄 Merging More Than Once

Yes, you can merge multiple times! Each time you merge `dev` into `main`, it will bring in only the changes that haven't been merged yet.

---

Happy coding and version-controlling! 🐱‍💻✨
