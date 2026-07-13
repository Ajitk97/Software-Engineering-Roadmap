# git init

## Defination

'git init initialise the new git repository in the current directry of our local system'

## Why do we need it?

'without initializing the repository, git cannot track version of files'

## Syntax

git init

## Command breakdown

| Part | Meaning |
|------|---------|
| git  | git program |
| init | initialize the new repository |

## What happens internally?

when the command is executed:

-git create a hidden .git folder.
-This folder stores commit history.
-It store branches.
-It stores configuration.
-It stores git object.

## Example

Current folder:
Projec/

After running 

'''bash
git init
'''

Project/
.git/

## Real project example

We initialize the repository before pushing Software-Roadmap Project o github.

## Common erros

Repositories already initialize

## Reason

The folder already contains .git directory.

## Interview question

What does git init do?
Ans: It creates a .git hidden directory that enables git version control.

## Revision

- Creates `.git`
- Starts version control
- Required before the first commit

## Things I Learned While Doing It

- `git init` only creates the repository locally.
- It does **not** create a GitHub repository.
- After `git init`, we still need:
  - `git add`
  - `git commit`
  - `git remote add origin`
  - `git push`
- GitHub authentication is separate from `git init`.