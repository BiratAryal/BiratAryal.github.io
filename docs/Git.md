# 🧠 Git Commands Cheat Sheet

---

## 📌 Git Configuration

| Command                                          | Description                        |
| ------------------------------------------------ | ---------------------------------- |
| `git config --global user.name "Birat Aryal"`    | Set your name (used in commits)    |
| `git config --global user.email "Email address"` | Set your email                     |
| `git config --list`                              | List all Git config values         |
| `git config --global core.editor code`           | Set default editor (e.g., VS Code) |

---
## 📌 Git Global Configuration

---

## 📁 Initialize & Clone

| Command                    | Description                     |
| -------------------------- | ------------------------------- |
| `git init`                 | Initialize a new Git repository |
| `git clone <url>`          | Clone an existing repo          |
| `git clone <url> <folder>` | Clone into a specific folder    |

---
## 📂 Project Setup Steps

| Step | Command                                                          | Description                                                |
| ---- | ---------------------------------------------------------------- | ---------------------------------------------------------- |
| 1️⃣  | `echo "# Automation" >> README.md`                               | Creates a `README.md` file with the title "Automation".    |
| 2️⃣  | `git init`                                                       | Initializes a new Git repository in the current directory. |
| 3️⃣  | `git add README.md`                                              | Stages the `README.md` file for the first commit.          |
| 4️⃣  | `git commit -m "first commit"`                                   | Commits the staged file with a message.                    |
| 5️⃣  | `git branch -M master`                                           | Renames the default branch to `master`.                    |
| 6️⃣  | `git remote add origin git@github.com:BiratAryal/Automation.git` | Sets the remote repository URL.                            |
| 7️⃣  | `git push -u origin master`                                      | Pushes the code to GitHub and sets upstream tracking.      |

---
## 🔍 Check Status & Logs

| Command             | Description                         |
| ------------------- | ----------------------------------- |
| `git status`        | Show changed files & staging status |
| `git log`           | View commit history                 |
| `git log --oneline` | View compact commit history         |
| `git diff`          | Show unstaged changes               |
| `git diff --staged` | Show staged changes                 |

---

## ➕ Add & Commit Changes

|Command|Description|
|---|---|
|`git add <file>`|Stage a specific file|
|`git add .`|Stage all modified files|
|`git commit -m "message"`|Commit with a message|
|`git commit -am "message"`|Add & commit tracked files only|

---

## ⬆️ Push & ⬇️ Pull

|Command|Description|
|---|---|
|`git push`|Push changes to remote|
|`git push -u origin <branch>`|Push and set upstream|
|`git pull`|Fetch and merge from remote|
|`git fetch`|Only fetch, don’t merge|
|`git remote -v`|Show remote URLs|

---

## 🌿 Branching

|Command|Description|
|---|---|
|`git branch`|List local branches|
|`git branch <name>`|Create a new branch|
|`git checkout <branch>`|Switch to a branch|
|`git checkout -b <branch>`|Create & switch branch|
|`git branch -d <branch>`|Delete a branch|
|`git merge <branch>`|Merge another branch into current|

---

## 💥 Undo / Reset / Revert

|Command|Description|
|---|---|
|`git restore <file>`|Discard changes in a file|
|`git restore --staged <file>`|Unstage a file|
|`git reset HEAD~1`|Undo last commit, keep changes|
|`git revert <commit>`|Create a new commit that undoes an old one|
|`git reset --hard`|Remove all local changes (⚠️ irreversible)|

---

## 🔍 Stash Changes

|Command|Description|
|---|---|
|`git stash`|Save changes temporarily|
|`git stash list`|List stashed changes|
|`git stash apply`|Reapply last stash|
|`git stash drop`|Delete the latest stash|

---

## 🔗 Tagging

|Command|Description|
|---|---|
|`git tag`|List all tags|
|`git tag <name>`|Create a lightweight tag|
|`git tag -a <name> -m "msg"`|Annotated tag|
|`git push origin <tag>`|Push tag to remote|

---

## 🤝 Collaborating (Remote)

|Command|Description|
|---|---|
|`git remote add origin <url>`|Add a new remote|
|`git push origin --tags`|Push all tags to remote|
|`git remote remove origin`|Remove remote|

---

## 🧪 Misc & Utilities

|Command|Description|
|---|---|
|`git show <commit>`|Show details of a commit|
|`git blame <file>`|Show who modified each line|
|`git clean -fd`|Remove untracked files & folders|
|`git reflog`|Log of all HEAD movements (recover lost commits)|

---

## 🧭 Common Workflows

### ✅ Feature Branch Workflow

```bash
git checkout -b feature/xyz
# work & commit
git push origin feature/xyz
```

### 🚀 Release Workflow

```bash
git checkout -b release/v1.0
git merge develop
```

### 🐞 Hotfix Workflow

```bash
git checkout -b hotfix/bug-123 main
# fix & commit
git push origin hotfix/bug-123
```

---