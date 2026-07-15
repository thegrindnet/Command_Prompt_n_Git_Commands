# Command Line and Git Commands

A simple reference guide for basic terminal, Git, and GitHub commands.

## Terminal Commands

| Command               | What it does                                         |
| --------------------- | ---------------------------------------------------- |
| `dir`                 | Shows files and folders in Windows Command Prompt    |
| `ls`                  | Shows files and folders in Git Bash, macOS, or Linux |
| `cd <folder-name>`    | Opens a folder                                       |
| `cd ..`               | Goes back one folder                                 |
| `mkdir <folder-name>` | Creates a folder                                     |
| `touch <filename>`    | Creates a file in Git Bash, macOS, or Linux          |
| `rm <filename>`       | Deletes a file                                       |
| `rm -r <folder-name>` | Deletes a folder and everything inside it            |
| `code .`              | Opens the current folder in Visual Studio Code       |

## Basic Git Commands

| Command                   | What it does                  |
| ------------------------- | ----------------------------- |
| `git init`                | Starts Git in a project       |
| `git status`              | Shows changed files           |
| `git add .`               | Stages all changes            |
| `git add <filename>`      | Stages one file               |
| `git commit -m "message"` | Saves staged changes          |
| `git log --oneline`       | Shows commit history          |
| `git push`                | Uploads commits to GitHub     |
| `git pull`                | Downloads changes from GitHub |

## Connect a Project to GitHub

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <repository-url>
git push -u origin main
```

## Daily Git Workflow

```bash
git status
git add .
git commit -m "Describe your changes"
git push
```

## Branch Commands

| Command                       | What it does                            |
| ----------------------------- | --------------------------------------- |
| `git branch`                  | Shows branches                          |
| `git switch -c <branch-name>` | Creates and opens a branch              |
| `git switch <branch-name>`    | Switches branches                       |
| `git merge <branch-name>`     | Merges a branch into the current branch |
| `git branch -d <branch-name>` | Deletes a merged branch                 |

## Undo Commands

| Command                           | What it does                          |
| --------------------------------- | ------------------------------------- |
| `git restore <filename>`          | Discards unstaged file changes        |
| `git restore --staged <filename>` | Removes a file from staging           |
| `git revert <commit-hash>`        | Reverses a commit safely              |
| `git reset --hard HEAD~1`         | Deletes the latest commit and changes |

> **Warning:** Be careful with `rm -r` and `git reset --hard`. They can permanently delete work.

## Git Stash

| Command          | What it does                      |
| ---------------- | --------------------------------- |
| `git stash`      | Temporarily saves unfinished work |
| `git stash pop`  | Restores the saved work           |
| `git stash list` | Shows saved stashes               |

## Remote Commands

| Command                | What it does                    |
| ---------------------- | ------------------------------- |
| `git remote -v`        | Shows the GitHub repository URL |
| `git fetch`            | Downloads remote information    |
| `git pull origin main` | Downloads and merges changes    |
| `git push origin main` | Uploads the main branch         |

## `.gitignore`

Create a `.gitignore` file to prevent Git from tracking certain files.

Example:

```gitignore
node_modules/
.env
dist/
```
