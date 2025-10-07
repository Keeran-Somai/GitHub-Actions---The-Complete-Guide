
# Git Guide Project

Welcome to the Git Guide Project! This repository contains a comprehensive HTML guide to Git, designed to help users of all levels understand and master version control with Git. Whether you're a beginner or an experienced developer, this guide provides practical examples, workflows, and tips to improve your productivity.

---

## Table of Contents

- [Git Guide Project](#git-guide-project)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Installation](#installation)
  - [How to Use](#how-to-use)
  - [Project Structure](#project-structure)
  - [Common Git Commands](#common-git-commands)
  - [Branching Strategies](#branching-strategies)
  - [Undoing Changes](#undoing-changes)
  - [Using .gitignore](#using-gitignore)
  - [Advanced Workflows](#advanced-workflows)
  - [Troubleshooting](#troubleshooting)
  - [Contributing](#contributing)
  - [FAQ](#faq)
  - [Helpful Resources](#helpful-resources)

---

## Features

- Overview of Git and version control concepts
- Step-by-step guide to common Git commands
- Typical workflow examples for solo and team projects
- Branching strategies for feature development and collaboration
- Undoing changes and recovering lost work
- Using `.gitignore` to manage ignored files
- Advanced Git tips and tricks
- Cheatsheet for quick reference
- Troubleshooting common issues
- Contribution guidelines

---

## Installation

1. Clone this repository:
	 ```bash
	 git clone https://github.com/Keeran-Somai/GitHub-Actions---The-Complete-Guide.git
	 ```
2. Navigate to the `sectionOne` directory:
	 ```bash
	 cd "GitHub Actions The Complete Guide/sectionOne"
	 ```
3. Open `index.html` in your preferred web browser.

---

## How to Use

Open `index.html` in your browser to view the guide. The guide is organized into sections covering everything from basic commands to advanced workflows. You can edit or extend the guide as needed for your team or personal use.

---

## Project Structure

- `index.html` - Main HTML guide for Git usage
- `.gitignore` - Example ignore file for common patterns
- `README.md` - This documentation file

---

## Common Git Commands

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a new Git repository |
| `git clone <url>` | Clone a remote repository |
| `git status` | Show the working directory status |
| `git add <file>` | Stage changes for commit |
| `git commit -m "message"` | Commit staged changes |
| `git log` | View commit history |
| `git branch` | List branches |
| `git checkout <branch>` | Switch branches |
| `git merge <branch>` | Merge a branch into current |
| `git pull` | Fetch and merge from remote |
| `git push` | Push changes to remote |

---

## Branching Strategies

- **Feature Branches:** Create a branch for each new feature or bugfix.
- **Main/Development Branches:** Keep `main` or `master` stable; use `develop` for ongoing work.
- **Pull Requests:** Merge changes via pull requests for code review.
- **Release Branches:** Prepare releases in dedicated branches.

Example:
```bash
git checkout -b feature/my-new-feature
```

---

## Undoing Changes

- Unstage a file: `git reset <file>`
- Discard changes: `git checkout -- <file>`
- Amend last commit: `git commit --amend`
- Recover lost commits: `git reflog`

---

## Using .gitignore

The `.gitignore` file tells Git which files or folders to ignore in a project. This is useful for excluding files like build output, logs, or sensitive information.

Example:
```
node_modules/

*.log
.env
```

---

## Advanced Workflows

- **Interactive Rebase:** `git rebase -i HEAD~n` to edit, squash, or reorder commits
- **Stash Changes:** `git stash` to save work-in-progress
- **Cherry-pick:** `git cherry-pick <commit>` to apply a specific commit
- **Bisect:** `git bisect start` to find the commit that introduced a bug
- **Tagging:** `git tag v1.0.0` to create a tag

---

## Troubleshooting

- **Merge Conflicts:**
	- Resolve conflicts in files, then run `git add <file>` and `git commit`.
- **Detached HEAD:**
	- Checkout a branch or create a new one to save changes.
- **Accidentally Deleted Branch:**
	- Recover with `git reflog` and `git checkout -b <branch> <commit>`.
- **Untracked Files Not Ignored:**
	- Check `.gitignore` patterns and file locations.

---

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a new branch for your feature or fix
3. Commit your changes with clear messages
4. Open a pull request describing your changes

---

## FAQ

**Q: How do I undo my last commit?**
A: Use `git reset --soft HEAD~1` to keep changes staged, or `git reset --hard HEAD~1` to discard them.

**Q: How do I ignore files in all my projects?**
A: Set up a global `.gitignore` with:
```bash
git config --global core.excludesfile ~/.gitignore_global
```

**Q: How do I see who changed a line?**
A: Use `git blame <file>`.

**Q: How do I recover a deleted branch?**
A: Use `git reflog` to find the commit and recreate the branch.

---

## Helpful Resources

- [Official Git Documentation](https://git-scm.com/doc)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)
- [GitHub Learning Lab](https://lab.github.com/)
- [Pro Git Book](https://git-scm.com/book/en/v2)

---

