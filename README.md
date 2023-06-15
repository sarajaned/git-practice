# git-practice

Anyone who completes this projects shows they can...

- Fork and Clone a repo
- understand git branching locally
- properly use git commands such as `status`, `add`, `commit` and `push`
- create `pull requests` (PR's) for code reviews

## Introduction

In this guide you will learn the basics of working with Git and Github and
also understand basic git workflow.

Project MVP is achieved by opening a PR requesting to merge your `name branch`
into `main` branch.

## Prerequisites

You should have git (Linux / Mac) or GitBash (Windows) installed and setup first
before you continue on.

Make sure you follow this first time setup so that git knows who you are, if not
git will ask you to set this up on your first commit

[Git First Time Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

The first thing you should do when you install Git is to set your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating:

```bash
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

## Instruction

- [ ] Please fork and clone this repository
- [ ] Create a new branch and name it with your name eg `john-doe`
- [ ] Create a new "Hello World" project using your language of choice such as
Python, Java, JavaScript, Ruby or even bash script.
- [ ] View the `status` of the git repo, `add` your changes to staging, view the status
of the repo again. Once happy with the status of the repo, `commit` your changes.
- [ ] `push` your changes up into `Github`
- [ ] Open a `pull request` (PR) setting your `name branch` as the branch to `merge`
into your `main` branch

## Git reference

### Staging Changes

```bash
git add .
```
Add all changed files and folder, in the current folder you are in, into the 
`staging` area

NOTE: `.` (dot) represents the current directory / folder that you are in.

```bash
git add ./filename [file2, file3, ...]
```
Add individual file(s) to the staging area.

### Commiting Changes

```bash
git commit -m "commit message"

# For multi line commmits
git commit -m "commit type: basic summary

details about the changes here"
```

Optoinal reading: [Semantic Commits](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716)

When you commit code, you need to create a message, these messages are very 
useful for your self and others to understand changes that were made in the code
at the specific point in time. This is really useful for when you want to 
undo changes you made in your project.

### View Repo Status

```bash
git status
```
View the current state that your repo is in. Shows whats in staging, changes and
other outstanding items.

### Pushing Changes

```bash
# replace <branch> with your branch name eg. git push origin main
git push origin <branch>
```
Push code back up to Github in the specified branch.

### Branching

```bash
# replace <branch-name> with a branch name eg. john-doe
git checkout -b <branch-name>
```
Create a new branch and move into it.

### Viewing Branches

```bash
git branch
```
Shows local branches available along with current working branch.

```bash
git branch -av
```
Shows all branches in the repo both local and remote.

### Moving Between Branches

```bash
git checkout <existing-branch>
```
Change your current working branch, to another branch that already exists

### Git Log

```bash
git log
```
Show the history of the git repo (project)

### Git Manual

```bash
man git
```
