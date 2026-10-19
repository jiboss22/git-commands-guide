# A Guide to Git Commands

## Introduction
Git is a tool that tracks changes to your files. Every time you
make a commit, Git saves a snapshot of your project, so you can see what
changed and go back to an older version if something breaks. Git works on
your own computer, and GitHub is a website where you can store your
projects online and share them with other people.

### Why Use Git?
- You can go back to an earlier version if you make a mistake.
- Several people can work on the same project without overwriting each other.
- Your code is backed up on GitHub, so you won't lose it if your computer breaks.

## Branches
A branch is a separate line of work in your project. It lets you try new
ideas or build a feature without changing the main version. When the work
is ready, you merge the branch back into main.

### Branch Commands
- `git branch` – lists all branches and shows which one you are on.
- `git checkout -b feature/name` – creates a new branch and switches to it.
- `git checkout main` – switches back to the main branch.
- `git merge feature/name` – adds the changes from a branch into the branch you are on.
- `git branch -d feature/name` – deletes a branch after it has been merged.

### Example
```
git checkout -b feature/new-section
git add guide.md
git commit -m "Add new section"
git checkout main
git merge feature/new-section
```