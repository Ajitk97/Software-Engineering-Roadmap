# Below are the GIT status with their meaning

## From now on, whenever you see git status, your brain should think:

|Output |	Meaning |
-------- -----------
- Untracked  files |	Git doesn't know about these files yet.
- Changes not staged for commit	| Git knows these files, but the latest changes haven't been staged.
- Changes to be committed	| These changes are staged and will be included in the next commit.
- Nothing to commit, working tree clean |	Working Directory, Staging Area, and Local Repository are synchronized.


## GIT File can be in 5 status

Untracked
   ↓
Tracked
   ↓
Modified
   ↓
Staged
   ↓
Committed

1. Untracked

Definition:
A new file that Git has never seen before.

Example:

InterviewQuestions.md

You create it and press Ctrl + S.

Run:

git status

Output:

Untracked files:
    InterviewQuestions.md
2. Tracked

Definition:
A file that Git knows about.

A file becomes tracked after:

git add <filename>

or if it was already committed earlier.

Example:

Git.md
3. Modified

Definition:
A tracked file whose contents have changed after the last commit.

Example:

Git.md

Edit it and save.

git status

Output:

Changes not staged for commit:

modified: Git.md
4. Staged

Definition:
A modified/new file that has been added to the Staging Area.

Command:

git add Git.md

Output:

Changes to be committed:

modified: Git.md
5. Committed

Definition:
A staged file that has been saved permanently in the Local Repository.

Command:

git commit -m "Update Git notes"
Complete Lifecycle
Create File
      │
      ▼
Untracked
      │
git add
      ▼
Tracked + Staged
      │
git commit
      ▼
Committed
      │
Edit File
      ▼
Modified
      │
git add
      ▼
Staged
      │
git commit
      ▼
Committed


## Next Concept: git status Messages

There are 5 common messages you should know.

1. Untracked files
Untracked files:
    Student.md

Meaning: Git has never tracked these files.

2. Changes not staged for commit
Changes not staged for commit:
    modified: Git.md

Meaning: The file is tracked, but the latest changes are only in the Working Directory.

3. Changes to be committed
Changes to be committed:
    modified: Git.md

Meaning: The file is in the Staging Area and is ready for the next commit.

4. Nothing to commit, working tree clean
nothing to commit, working tree clean

Meaning:

No pending changes.
Working Directory = Staging Area = Local Repository.
5. Branch Ahead/Behind
Your branch is ahead of 'origin/main' by 1 commit.

Meaning: Your Local Repository has one or more commits that haven't been pushed.

Your branch is behind 'origin/main' by 2 commits.

Meaning: The Remote Repository has newer commits that your local repository doesn't have yet.