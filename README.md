# Git

Main reference: [MIT's missing semester](https://missing.csail.mit.edu/2020/version-control/).

## Building blocks
![git-uml.PNG](git-uml.png)

### Objects
An "object" is a blob, tree, or commit.
In Git all objects are content-addressed by their SHA-1 hash.

### Trees and blobs
In Git terminology, a file is called a "blob", and it’s just a bunch of bytes. A directory is called a “tree”, and it maps names to blobs or trees (so directories can contain other directories).

### Commits
Git models the history of a collection of files and folders within some top-level directory as a series of snapshots. In Git terminology, a file is called a "blob", and it’s just a bunch of bytes.
A directory is called a "tree", and it maps names to blobs or trees (so directories can contain other directories).
A snapshot is the top-level tree that is being tracked, Git calls these snapshots "commit"s.


## Git commands
The best way to interact with Git is via its command line interface.

### Basics
* `git status`: tells you what’s going on.
* `git add <filename>`: adds files to staging area.
* `git commit`: creates a new commit.
* `git log`: shows a flattened log of history.
* `git diff [<reference>] <filename>`: shows differences in a file between snapshots (or relative to the staging area if no revision is given).
* `git checkout <reference>`: moves HEAD to reference.
* `git branch <name>`: create branch.
* `git merge <reference>`: merges into current branch.

### Advanced
TODO: Add small description to each command.

* `git log --all --graph --decorate` or `git graph` (custom alias).
* `git mergetool`.
* `git reset`.
* `git revert`.
* `git add –p`.
* `git stash`.
* `git bisect`.
