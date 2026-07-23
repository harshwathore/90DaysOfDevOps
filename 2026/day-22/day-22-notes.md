# Day 22 - Git Notes

## 1. What is the difference between `git add` and `git commit`?

`git add` is used to move changes from the working directory to the staging area. It prepares the changes that should be included in the next commit.

`git commit` saves the staged changes permanently in the Git repository with a commit message. It creates a new snapshot of the project.

---

## 2. What does the staging area do? Why doesn't Git just commit directly?

The staging area acts as a temporary place where I can choose which changes should be included in the next commit.

Git does not commit directly because I may modify multiple files but only want to commit some of them. The staging area gives me control over what goes into each commit, helping keep the commit history clean and meaningful.

---

## 3. What information does `git log` show you?

`git log` shows the history of commits in the repository.

It includes:
- Commit ID (SHA hash)
- Author name
- Author email
- Date and time
- Commit message

This helps track who made changes, when they were made, and why.

---

## 4. What is the `.git/` folder and what happens if you delete it?

The `.git/` folder is the hidden folder that stores all Git metadata, including commits, branches, tags, logs, configuration, and the complete version history of the project.

If I delete the `.git/` folder, the project files will still exist, but Git will no longer recognize it as a Git repository. All commit history, branches, and Git tracking information will be lost.

---

## 5. What is the difference between a working directory, staging area, and repository?

### Working Directory
The working directory is where I create, edit, and delete project files. These changes are not yet tracked for the next commit.

### Staging Area
The staging area is a temporary area where I select the changes that should be included in the next commit using `git add`.

### Repository
The repository contains all committed versions of the project. Every commit is stored here permanently, allowing me to view history, compare versions, and restore previous states.