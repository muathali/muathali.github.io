---
title: "Git"
date: 2021-06-26T21:33:26-04:00
draft: false
---

Quick git facts to better understand how it works

Each file in your working directory can be in one of two states: tracked or untracked. Tracked files are files that were in the last snapshot;

They can be unmodified, modified, or staged. Untracked files are everything else – any files in your working directory that were not in your last snapshot and are not in your staging area. When you first clone a repository, all of your files will be tracked and unmodified because Git just checked them out and you haven’t edited anything.

Untracked basically `means that` Git sees a file you didn’t have in the previous snapshot (commit);

git add is a multipurpose command – you use it to begin tracking new files, to stage files, and to do other things like marking merge-conflicted files as resolved. It may be helpful to think of it more as “add this content to the next commit” rather than “add this file to the project

It’s best to have a clean working state when you switch branches. There are ways to get around this (namely, stashing and commit amending) that we’ll cover later on, in Stashing and Cleaning. This is an important point to remember: when you switch branches, Git resets your working directory to look like it did the last time you committed on that branch. It adds, removes, and modifies files automatically to make sure your working copy is what the branch looked like on your last commit to it.

The Golden Rule of Git: Never rebase shared commit

## Push an existing repository from the command line

```bash
git remote add origin repo-url.git
git branch -M main
git push -u origin main
```

## git remote

```bash
git remote [-v | --verbose]
git remote show origin
```

## git branch

```bash
git branch -a
git branch -vv # Show local branches
```

## git stash

```bash
git stash --include-untracked
git stash list
git stash apply
git stash clear
```
