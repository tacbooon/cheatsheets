# Git Cheat Sheet

## Table of Contents

- [Git Cheat Sheet](#git-cheat-sheet)
  - [Table of Contents](#table-of-contents)
  - [Repository](#repository)
    - [Create an empty repository](#create-an-empty-repository)
    - [Clone a repository](#clone-a-repository)
    - [Clone a repository and checkout a specific branch](#clone-a-repository-and-checkout-a-specific-branch)
    - [Clone a repository and its submodules recursively](#clone-a-repository-and-its-submodules-recursively)
    - [Create a shallow clone with a history truncated](#create-a-shallow-clone-with-a-history-truncated)
  - [Branch](#branch)
    - [Create a new branch which points to the current HEAD](#create-a-new-branch-which-points-to-the-current-head)
    - [Create a new branch which points to the current HEAD and switch to it](#create-a-new-branch-which-points-to-the-current-head-and-switch-to-it)
    - [Switch to a specific branch](#switch-to-a-specific-branch)
    - [Rename the current branch](#rename-the-current-branch)
    - [Rename a specific branch](#rename-a-specific-branch)
    - [Delete a branch](#delete-a-branch)
    - [Delete a branch forcelly](#delete-a-branch-forcelly)
    - [Show a list of local branches](#show-a-list-of-local-branches)
    - [Show a list of remote branches](#show-a-list-of-remote-branches)
  - [Tag](#tag)
    - [Create a tag](#create-a-tag)
    - [Create a tag with a message](#create-a-tag-with-a-message)
    - [Delete a tag](#delete-a-tag)
    - [Show a tag message and referenced object](#show-a-tag-message-and-referenced-object)
    - [Show a list of tags](#show-a-list-of-tags)
  - [Index](#index)
    - [Add files to the index](#add-files-to-the-index)
    - [Add only tracked files to the index](#add-only-tracked-files-to-the-index)
    - [Interactively choose hunks of patch and add them to the index](#interactively-choose-hunks-of-patch-and-add-them-to-the-index)
    - [Unstage files from the index](#unstage-files-from-the-index)
    - [Restore working tree files](#restore-working-tree-files)
    - [Move or rename a file](#move-or-rename-a-file)
    - [Remove files from both working tree and index](#remove-files-from-both-working-tree-and-index)
    - [Clean untracked files from the working tree](#clean-untracked-files-from-the-working-tree)
    - [Show what untracked files would be removed by clean](#show-what-untracked-files-would-be-removed-by-clean)
  - [Commit](#commit)
    - [Commit staged changes with a message](#commit-staged-changes-with-a-message)
    - [Commit all local changes](#commit-all-local-changes)
    - [Create an empty commit](#create-an-empty-commit)
    - [Create a fixup commit](#create-a-fixup-commit)
    - [Change the last commit](#change-the-last-commit)
    - [Change the last commit without changing its commit message](#change-the-last-commit-without-changing-its-commit-message)
    - [Reset the first commit](#reset-the-first-commit)
    - [Revert existing commits](#revert-existing-commits)
  - [Status](#status)
    - [Show working tree status](#show-working-tree-status)
    - [Show working tree status but ignores submodules](#show-working-tree-status-but-ignores-submodules)
    - [Show changes between the working tree and the index](#show-changes-between-the-working-tree-and-the-index)
    - [Show changes between commits](#show-changes-between-commits)
  - [History](#history)
    - [Show commit logs](#show-commit-logs)
    - [Show who changed what and when](#show-who-changed-what-and-when)
    - [Search commit messages](#search-commit-messages)
  - [Remote](#remote)
    - [Show a list of remote repositories](#show-a-list-of-remote-repositories)

## Repository

### Create an empty repository

```
git init
```

### Clone a repository

```
git clone URL
```

### Clone a repository and checkout a specific branch

```
git clone URL -b BRANCH
```

### Clone a repository and its submodules recursively

```
git clone --recurse-submodules URL
```

### Create a shallow clone with a history truncated

```
git clone --depth=1 URL
```

## Branch

### Create a new branch which points to the current HEAD

```
git branch BRANCH
```

### Create a new branch which points to the current HEAD and switch to it

```
git switch -c BRANCH
```

### Switch to a specific branch

```
git switch BRANCH
```

### Rename the current branch

```
git branch -m NEW_BRANCH
```

### Rename a specific branch

```
git branch -m OLD_BRANCH NEW_BRANCH
```

### Delete a branch

```
git branch -d BRANCH
```

### Delete a branch forcelly

```
git branch -D BRANCH
```

### Show a list of local branches

```
git branch
```

### Show a list of remote branches

```
git branch --remote
```

## Tag

### Create a tag

```
git tag TAG [COMMAND or OBJECT]
```

### Create a tag with a message

```
git tag -a TAG -m MESSAGE [COMMAND or OBJECT]
```

### Delete a tag

```
git tag -d TAG
```

### Show a tag message and referenced object

```
git show TAG
```

### Show a list of tags

```
git tag -l [PATTERN]
```

## Index

### Add files to the index

```
git add FILE...
```

### Add only tracked files to the index

```
git add -u [FILE...]
```

### Interactively choose hunks of patch and add them to the index

```
git add -p FILE...
```

### Unstage files from the index

```
git reset HEAD [FILE...]
```

### Restore working tree files

```
git restore FILE...
```

### Move or rename a file

```
git mv [-f] SOURCE DESTINATION
```

### Remove files from both working tree and index

```
git rm [-f] [-r] FILE...
```

### Clean untracked files from the working tree

```
git clean -fd [FILE]...
```

### Show what untracked files would be removed by clean

```
git clean -nd [FILE]...
```

## Commit

### Commit staged changes with a message

```
git commit [-m MESSAGE]
```

### Commit all local changes

```
git commit -a [-m MESSAGE]
```

### Create an empty commit

```
git commit --allow-empty [-m MESSAGE]
```

### Create a fixup commit

```
git commit --fixup=COMMIT
```

### Change the last commit

```
git commit --amend [-m MESSAGE]
```

### Change the last commit without changing its commit message

```
git commit --amend --no-edit
```

### Reset the first commit

```
git update-ref -d HEAD
```

### Revert existing commits

```
git revert COMMIT...
```

## Status

### Show working tree status

```
git status
```

### Show working tree status but ignores submodules

```
git status --ignore-submodules
```

### Show changes between the working tree and the index

```
git diff [FILE...]
```

### Show changes between commits

```
git diff FROM TO
```

## History

### Show commit logs

```
git log [-COUNT]
```

### Show who changed what and when

```
git blame FILE
```

### Search commit messages

```
git log -i -E --grep=PATTERN
```

## Remote

### Show a list of remote repositories

```
git remote -v
```
