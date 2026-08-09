Sure — here is the same content formatted as a ready-to-save **Markdown (`.md`) file**:

# Git Commands Cheat Sheet

## Basic Git Commands

| #  | Command                       | Description                                     |
| -- | ----------------------------- | ----------------------------------------------- |
| 1  | `git init`                    | Initializes a new Git repository                |
| 2  | `git add <file_name>`         | Adds a file to the staging area                 |
| 3  | `git commit -m "Message"`     | Saves staged changes as a commit                |
| 4  | `git log`                     | Shows the commit history                        |
| 5  | `git checkout <commit-code>`  | Switches to a specific commit                   |
| 6  | `git branch`                  | Lists all existing branches                     |
| 7  | `git switch <branch>`         | Switches to another branch                      |
| 8  | `git status`                  | Shows the current repository status             |
| 9  | `git diff`                    | Shows changes that have not been staged         |
| 10 | `git push -u origin <branch>` | Pushes a branch to the remote repository        |
| 11 | `git clone <url>`             | Clones a remote repository                      |
| 12 | `git pull origin <branch>`    | Fetches and merges changes from a remote branch |

---

## 1. Initialize Git Repository

```bash
git init
```

Initializes a new Git repository in the current directory.

---

## 2. Add File

```bash
git add <file_name>
```

Adds a specific file to the staging area.

To add all files:

```bash
git add .
```

---

## 3. Commit Changes

```bash
git commit -m "Message"
```

Creates a commit with a descriptive message.

Example:

```bash
git commit -m "Added login page"
```

---

## 4. View Commit History

```bash
git log
```

Displays the commit history.

For a shorter version:

```bash
git log --oneline
```

---

## 5. Checkout a Commit

```bash
git checkout <commit-code>
```

Switches to a specific commit.

Example:

```bash
git checkout a1b2c3d
```

> **Note:** `git checkout` can also be used for branches, but modern Git recommends `git switch` for switching branches.

---

## 6. View Branches

```bash
git branch
```

Lists all local branches.

The current branch is marked with `*`.

---

## 7. Switch Branch

```bash
git switch <branch>
```

Switches to an existing branch.

Example:

```bash
git switch main
```

### Create and Switch to a New Branch

```bash
git switch -c feature-login
```

---

## 8. Check Git Status

```bash
git status
```

Shows:

* Modified files
* New files
* Staged files
* Current branch
* Untracked files

---

## 9. View Changes

```bash
git diff
```

Shows changes that have not been staged.

To see staged changes:

```bash
git diff --staged
```

---

## 10. Push to Remote Repository

```bash
git push -u origin <branch>
```

Uploads your local branch to the remote repository.

Example:

```bash
git push -u origin main
```

After setting the upstream branch, you can usually use:

```bash
git push
```

---

## 11. Clone a Repository

```bash
git clone <url>
```

Downloads a remote repository to your local computer.

Example:

```bash
git clone https://github.com/user/project.git
```

Then enter the project directory:

```bash
cd project
```

---

## 12. Pull Changes

```bash
git pull origin <branch>
```

Downloads the latest changes from the remote repository and merges them into the current branch.

Example:

```bash
git pull origin main
```

---

# Common Git Workflow

## New Project

```bash
git init
git status
git add .
git commit -m "Initial commit"
git branch
git switch -c main
git push -u origin main
```

## Existing Project

```bash
git clone <url>
cd <project>
git status
git add .
git commit -m "Updated files"
git push origin main
```

## Get Latest Changes

```bash
git pull origin main
```

---

# Quick Reference

```bash
git init
git status
git add .
git commit -m "Message"
git log
git branch
git switch <branch>
git diff
git push -u origin <branch>
git clone <url>
git pull origin <branch>
```

> **Tip:** Modern Git generally recommends:
>
> * `git switch` → switching branches
> * `git restore` → restoring files
> * `git checkout` → still valid, but has multiple older uses

You can save this as **`git-commands.md`**.
