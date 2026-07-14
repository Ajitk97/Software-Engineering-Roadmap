# GIT

## What is GIT?
Definition

Git is a Distributed Version Control System (DVCS) used to track changes in source code and other files. It allows developers to manage different versions of a project, collaborate with team members, and restore previous versions whenever needed.

## Why was Git created?

Before Git, developers faced several problems:

Multiple developers overwrote each other's code.
There was no easy way to restore an older version of the project.
Teams struggled to track who changed what and when.
Collaboration became difficult as projects grew.

Git was created by Linus Torvalds in 2005 to solve these problems while developing the Linux kernel.

Pushed the code to Azure Repos.
Created a YAML pipeline.

Without Git, Azure DevOps Repos wouldn't have any project history to work with.

## Advantages of Git
- Tracks every change made to a project.
- Allows multiple developers to work simultaneously.
- Maintains complete version history.
- Makes collaboration easier.
- Enables branching and merging.
- Helps recover previous versions of the project.

# Interview Question

## What is Git?

Answer:

Git is a Distributed Version Control System that tracks changes in files and source code. It allows developers to maintain version history, collaborate with team members, and restore previous versions of a project when required.

## Things I Learned

Write this in your own words:

Git is not GitHub.
Git is installed on my local machine.
Git tracks changes locally.
GitHub and Azure DevOps are remote platforms that can store Git repositories.
Revision
Git = Version Control System
Created by Linus Torvalds (2005)
Tracks changes
Supports collaboration
Stores version history
Used with GitHub and Azure DevOps
Practical (5 minutes)

## Open Command Prompt and run:

git --version
Why?

This command checks whether Git is installed and displays the installed version.

## Command Breakdown

Part	Meaning
git	Starts the Git program
--version	Displays the installed Git version

Expected output:

git version 2.xx.x.windows.x

## To verify which github account is connected use the below command

- git remote -v

- git branch -vv. To check which is the local branch & which is the git hub branch connected.