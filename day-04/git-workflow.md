# Day 4 — Git Workflow & Branching

## Git Status

`git status` shows the current state of the working directory and staging area.

It tells us:
- Which branch we are on
- Which files have been modified
- Which files are staged
- Whether there is anything to commit

Example:

`git status`

## Git Add

`git add` moves selected changes from the working directory into the staging area.

Example:

`git add day-04`

## Git Commit

`git commit` saves a snapshot of the staged changes in Git.

Example:

`git commit -m "Update Day 4 notes"`

## Git Push

`git push` sends committed changes from the local computer to GitHub.

Local → GitHub

Example:

`git push`

## Git Pull

`git pull` brings the latest changes from GitHub to the local computer.

GitHub → Local

Example:

`git pull`

## Git Log

`git log --oneline` shows the commit history in a compact format.

Each commit contains:
- A unique commit ID
- A commit message

Example:

`git log --oneline`

## Git Diff

`git diff` shows changes made to files that have not been committed.

It helps us review what changed before committing.

Example:

`git diff`

In the output:
- `-` shows removed/old content
- `+` shows added/new content

## Git Restore

`git restore <filename>` can discard uncommitted changes and restore the file to its last committed version.

Example:

`git restore day-04/git-workflow.md`

Important:
This can remove uncommitted changes, so it should be used carefully.

## Git Branch

A Git branch is an independent line of development for the same project.

It allows developers to work on new features without directly affecting the main branch.

Example:

`main`
`practice`

## Git Branch Command

`git branch` shows the branches in the repository.

The `*` identifies the current branch.

Example:

`git branch`

## Git Switch

`git switch <branch>` changes the current working branch.

Example:

`git switch practice`

To return to main:

`git switch main`

## Git Merge

`git merge <branch>` brings the changes from another branch into the current branch.

Example:

`git switch main`
`git merge practice`

This means the changes from `practice` are merged into `main`.

## Git Workflow

A basic Git workflow is:

Make changes
↓
git status
↓
git add
↓
git commit
↓
git push
↓
Verify on GitHub

## Branch Workflow

For developing a new feature:

Create branch
↓
Switch to branch
↓
Make changes
↓
Stage changes
↓
Commit changes
↓
Switch to main
↓
Merge branch
↓
Push to GitHub