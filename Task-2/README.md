# Using .gitignore and Tracking Files

## Overview
This repository demonstrates the use of a `.gitignore` file to exclude specific files and directories from being tracked by Git.

## Steps Performed

1. **Initialize the Repository**
   - Ran `git init` to initialize a new Git repository.
   - Verified the repository status using `git status`.

2. **Create a `.gitignore` File**
   - Created a `.gitignore` file and added the patterns:
     
3. **Add Files and Directories**
   - Created the following files and directories:
     - `.env` file to simulate sensitive information.
     - `output/` directory with a file `details.txt` inside it.
     - `tracked_file.txt` to test file tracking.

4. **Verify .gitignore Behavior**
   - Ran `git status` to confirm the `.env` file and `output/` directory were ignored, while `tracked_file.txt` was listed as untracked:
     #### Output:
     ```
     Untracked files:
      .gitignore
      tracked_file.txt
     ```

5. **Add and Commit Tracked Files**
   - Added and committed the tracked file:
     ```sh
     git add .
     git commit -m "created gitignore & some other file to test it[ADD]"
     ```

6. **Test Ignored Files**
   - Attempted to add the `.env` file to confirm it was ignored:
     ```sh
     git add .env
     ```
     Output:
     ```
     The following paths are ignored by one of your .gitignore files:
     .env
     hint: Use -f if you really want to add them.
     ```

7. **Verify Commit History**
   - Verified the commit history using:
     ```sh
     git log --oneline --graph
     ```

## Repository Structure
```
Task-2/
├── .gitignore
├── tracked_file.txt
├── .env (ignored)
└── output/ (ignored)
    └── details.txt
```
