#  GitHub 

<p align="center">
  <b>Managing and Sharing Projects Online</b><br>
  Technical Writing (TW) | MNIT Jaipur
</p>

---

##  Table of Contents
1. Introduction
2. Git vs GitHub
3. Key Features
4. Creating a Repository
5. Connecting Local and Remote Repositories
6. Uploading and Downloading Projects
7. Branches and Pull Requests
8. Collaboration Tools
9. Security and Best Practices
10. Learning Outcome

## 1. Introduction

GitHub is an online platform for hosting Git repositories and collaborating on software projects. It allows developers to share code, maintain project history, review changes, and work together.

## 2. Git vs GitHub

| Git | GitHub |
|---|---|
| Version control system | Hosting and collaboration platform |
| Works locally | Provides remote repositories |
| Tracks file changes | Shares and reviews projects |
| Maintains commits and branches | Supports pull requests and Issues |

## 3. Key Features

- **Repositories:** Store and organize project files.
- **Pull Requests:** Propose and review changes.
- **Issues:** Track bugs and tasks.
- **Forking:** Create a separate copy of another repository.
- **GitHub Projects:** Organize and track project progress.
- **Code Review:** Review contributions before merging.

## 4. Creating a Repository

Steps to create a GitHub repository:

1. Visit https://github.com/.
2. Sign in to your account.
3. Select **New repository**.
4. Enter a repository name.
5. Choose Public or Private visibility.
6. Select **Create repository**.

A README file can be added to introduce the project and explain its purpose.

## 5. Connecting Local and Remote Repositories

Connect a local Git repository to GitHub:

```bash
git remote add origin REPOSITORY_URL
```

Check the remote connection:

```bash
git remote -v
```

Here, `origin` is the conventional name given to the remote repository.

## 6. Uploading and Downloading Projects

**Upload a project to GitHub:**

```bash
git branch -M main
git push -u origin main
```

**Clone a repository:**

```bash
git clone REPOSITORY_URL
```

**Download and integrate remote updates:**

```bash
git pull
```

**Fetch remote updates without integrating them:**

```bash
git fetch origin
```

## 7. Branches and Pull Requests

Branches allow developers to work independently on new features.

A Pull Request (PR) is used to propose changes for review before merging them into another branch.

**Typical Pull Request Process:**
1. Create a feature branch.
2. Make changes and commit them.
3. Push the branch to GitHub.
4. Open a Pull Request.
5. Review and merge the changes.

## 8. Collaboration Tools

| Tool | Purpose |
|---|---|
| Issues | Track bugs and tasks |
| Pull Requests | Review proposed changes |
| Fork | Create a separate repository copy |
| Projects | Organize project activities |
| Actions | Automate workflows and testing |

## 9. Security and Best Practices

- Keep passwords and API keys private.
- Use appropriate repository permissions.
- Write clear commit messages.
- Maintain an updated README.
- Review code before merging.
- Use `.gitignore` for unnecessary local files.

## 10. Learning Outcome

Through practical exercises, I learned how to create GitHub repositories, connect local projects, upload and clone repositories, and collaborate using branches and pull requests.

---

<p align="center">
  <b>Technical Writing | MNIT Jaipur</b>
</p>