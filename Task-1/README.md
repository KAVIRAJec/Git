# Git Task - Initialize, Commit, and Branch Basics

## Overview
This repository demonstrates the basics of Git, including initializing a repository, creating and committing files, branching, and merging.

## Steps Performed

1. **Initialize the Repository**
   - Ran `git init` to initialize a new Git repository.
   - Verified the repository status using `git status`.

2. **Create and Commit Files in the Master Branch**
   - Created `index.html` and added the content
   - Staged and committed the file:
     ```sh
     git add index.html
     git commit -m "initialized index.html[ADD]"
     ```
   - Created styles.css & included in HTML then added the content:
     
   - Staged and committed the file:
     ```sh
     git add .
     git commit -m "created styles & included in index[ADD]"
     ```

3. **Create and Switch to a New Branch**
   - Created a new branch named `feature-update` and switched to it:
     ```sh
     git checkout -b feature-update
     ```

4. **Edit and Commit Changes in the New Branch**
   - Edited index.html in the `feature-update` branch.
   - Staged and committed the changes:
     ```sh
     git add index.html
     git commit -m "added feature update in index.html[CHANGE]"
     ```

5. **Merge the Branch Back to Master**
   - Switched back to the `master` branch:
     ```sh
     git checkout -b master
     ```
   - Merged the `feature-update` branch into `master`:
     ```sh
     git merge feature-update
     ```

6. **Verify the Commit History**
   - Verified the commit history using:
     ```sh
     git log --oneline --graph
     ```

## Repository Structure

```
git/
└── Task-1/
  ├── index.html
  └── styles.css
```
