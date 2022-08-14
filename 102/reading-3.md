[Home](../README.md)

# Reading Assignment 3

## What is Git?

Git is a distributed version control system (DVCS). A version control system tracks changes made to files in a specified location across time. It can be local on your machine, centralized in a single server somewhere, or distributed with multiple copies of files hosted in different places to eliminate the single point of failure.  Git allows different people to collaborate on work and track who made what changes. This is especially helpful in identifying at what point a piece of code started or stopped working, and what specific change caused it!

When using Git, you have a working directory, where you make most changes, a staging area where changes are prepared to sync with with the main body, and a repository (or repo) which contains the finalized changes to a document.  `git status` in the terminal will tell you what files, if any, have pending changes. Once changes are made to a file, use `git add FILENAME.EXTENSION` to add the desired files to the staging area. From there, you use `git commit` to commit all of the staged changes to the repo. If working in a repository cloned from GitHub, use `git push` to sync the changes made in the local repo with the GitHub repo.

