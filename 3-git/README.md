#  Git – Version Control System

<p align="center">
  <b>Tracking and Managing Project Changes</b><br>
  Technical Writing (TW) | MNIT Jaipur
</p>

---

##  Table of Contents
1. Introduction
2. Need for Version Control
3. Key Features of Git
4. Installation and Configuration
5. Creating a Repository
6. Basic Git Workflow
7. Important Git Commands
8. Branching and Merging
9. Merge Conflicts
10. Best Practices
11. Learning Outcome

## 1. Introduction

Git is a distributed version control system used to track changes in files and manage software development projects. It allows developers to maintain project history and work on different features independently.

## 2. Need for Version Control

Version control helps developers:
- Track modifications made to files.
- Recover previous versions.
- Identify who made changes and when.
- Manage contributions from multiple developers.
- Avoid losing important project updates.

## 3. Key Features of Git

- **Distributed System:** Every clone contains repository history.
- **Commit History:** Records project changes.
- **Branching:** Supports independent development.
- **Merging:** Combines changes from different branches.
- **Offline Support:** Basic Git operations work locally.

## 4. Installation and Configuration

Download Git from the official website:

https://git-scm.com/downloads

Check installation:

```bash
git --version
```

Configure username and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Verify configuration:

```bash
git config --global --list
```

## 5. Creating a Repository

Create a project folder and initialize Git:

```bash
mkdir my-project
cd my-project
git init
```

Git creates a hidden `.git` directory to store repository information and history.

## 6. Basic Git Workflow

Git works through three main areas:

- **Working Directory:** Where files are created or modified.
- **Staging Area:** Where changes are selected for the next commit.
- **Repository:** Stores committed project history.

The basic workflow is:

**Edit → Stage → Commit**

## 7. Important Git Commands

| Command | Purpose |
|---|---|
| `git status` | Check repository status |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Record changes |
| `git log` | View commit history |
| `git log --oneline` | View compact history |
| `git diff` | Compare file changes |
| `git branch` | List branches |
| `git switch branch-name` | Switch branches |
| `git merge branch-name` | Merge branches |
| `git restore file-name` | Discard unstaged changes in a tracked file |

## 8. Branching and Merging

A branch is an independent line of development. It allows developers to work on new features without directly changing the main branch.

Create and switch to a branch:

```bash
git switch -c feature-login
```

Merge it into the main branch:

```bash
git switch main
git merge feature-login
```

## 9. Merge Conflicts

A merge conflict occurs when Git cannot automatically combine changes from different branches.

**Resolution steps:**
1. Open the conflicting file.
2. Decide which changes to keep or combine.
3. Remove conflict markers.
4. Stage the resolved file.
5. Complete the merge.

## 10. Best Practices

- Write meaningful commit messages.
- Commit changes regularly.
- Use descriptive branch names.
- Review changes before committing.
- Keep sensitive files out of repositories.
- Maintain a clear project history.

## 11. Learning Outcome

Through practical exercises, I learned how to initialize repositories, track files, create commits, inspect project history, and manage branches and merge conflicts using Git.

---

<p align="center">
  <b>Technical Writing | MNIT Jaipur</b>
</p>