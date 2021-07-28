# Git scripts I use a bunch

## `git-commit-message`
##### Usage:  `git commit-message [-a] [-h] [-l] [-p] <message>`

When creating a commit, optionally stage all files beforehand and/or push to remote (optionally with lease)

### Options/Flags
```
[-h] display help and usage
[-A] stage all changed files before committing
[-l] push using force-with-lease after committing
[-p] push after committing
```

---

## `git-open`
##### Usage:  `git-open <branch-name>`

When opening a branch, first stash any changed files, then change to master and pull from remote before opening the branch.

---

## `git-push-up`
##### Usage:  `git push-up [-h] [-f] [-l]`

A short command to push changes to `origin/<branch-name>` without having to remember what the branch name, and optinoally force or force with lease.

### Options/Flags
```
[-h] display help and usage
[-f] push using --force
[-l] push using --force-with-lease
```

---

## `git-rebase-master`
##### Usage:  `git rebase-master [-h] [-i] [-p] [-s]`

A quick way to optionally stage all files and push to remote (including with lease) when creating a new commit.

### Options/Flags
```
[-h] display help and usage
[-i] use an interactive rebase with master
[-p] push using force-with-lease after rebasing
[-s] stash changes before and pop after
```