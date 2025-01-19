---
title: gitscussion
layout: appleII
---
a discussion of git
===================

what is git?
------------

- git is a system of snapshots.

- git is a system of ways to get from one snapshot to another.

git is a graph; the nodes are snapshots, the edges are ways to get
from one snapshot to another

```
git log --graph --oneline
```

what are the two modes of operation of git?
-------------------------------------------

- a work area with savepoints / checkpoints so you don't lose your
  work and so you can go back to a version that worked. Usually only
  you care about this.

- the record of versions (the permanent record). Your team cares about
  this, and so do people outside your team.

what are the two modes of merging in git?
-----------------------------------------

- `git-merge` (interleave commits based on time)

- `git-rebase` (apply commit after getting the latest code)

observations:
-------------

- in general, probably should rebase

- do not rewrite history after pushing to github (exception: your own
  private branches)

- git makes it hard to lose your work

References Make Commits Reachable
---------------------------------

- branches

- tags

git grab bag
------------

- `git stash`

- `git-gc`

Bibliography:

[Understanding the Git Workflow](https://sandofsky.com/blog/git-workflow.html)

[Think Like (a) Git](http://think-like-a-git.net/)
