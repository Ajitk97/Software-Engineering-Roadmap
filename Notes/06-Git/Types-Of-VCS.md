# TYPES OF VERSION CONTROL SYSTEM.

## There are 3 Types of Version Control Systems
1. Local VCS

↓

2. Centralized VCS

↓

3. Distributed VCS (Git)

We'll understand them one by one.

1. Local Version Control System (LVCS)
Definition

- A Local Version Control System stores all version history only on your own computer.

There is no server.

No GitHub.

No Azure DevOps.

Everything stays on one PC.

## Architecture
- Developer

↓

- Local Computer

↓

- Version History
Example

Suppose you're writing

Notes.docx

Your computer keeps:

Version 1

Version 2

Version 3

But they're only available on your computer.

## Advantages
Simple
Fast
Doesn't require internet
Disadvantages

If your computer crashes...

❌ Everything is lost.

No backup.

No collaboration.

## 2. Centralized Version Control System (CVCS)

Developers realized:

"Keeping everything on one PC is risky."

So they created a central server.

Architecture
           Server

      Project Repository

        /     |      \

Developer Developer Developer

Now every developer connects to the same server.

Example

Imagine Microsoft has one server.

All developers download code from it.

When someone changes code,

they upload it back to the server.

Advantages
Easier collaboration.
One central copy.
Better than Local VCS.
Disadvantages

Suppose the server crashes.

Server

💥 Crash

Nobody can work.

Everything stops.

This is called a Single Point of Failure.

## 3. Distributed Version Control System (DVCS)

This is where Git comes in.

Git says:

"Why should only the server have the complete project history?"

Instead...

Every developer gets a complete copy of the repository.

## Architecture
               GitHub

            Full Repository

            /     |      \

Developer Developer Developer

Each developer also has

a complete repository.

Notice something.

Each developer has:

Complete source code
Complete commit history
Complete branches

Everything.

Real Example

Your laptop:

Software-Engineer-Roadmap

contains:

.git

That hidden folder contains the repository.

GitHub also contains the repository.

Both have history.

That's why Git is called Distributed.

What happens if GitHub goes down?

Suppose GitHub is unavailable.

Can you still work?

✅ Yes.

You can:

Edit code.
Commit.
Create branches.
View history.

The only thing you can't do is:

git push

because the remote server is unavailable.

This is a huge advantage of Git.

Comparison Table
Feature	Local VCS	Centralized VCS	Distributed VCS (Git)
History Stored	Local PC	Server	Every Developer
Internet Required	No	Yes	Only for Push/Pull
Collaboration	No	Yes	Yes
Backup	No	Server Only	Every Developer
Server Failure	No Server	Work Stops	Developers Can Continue
Real Project Example

Think about your Azure DevOps project.

When you cloned or initialized your repository:

EcomDevApi

Your development machine had:

.git

Azure DevOps also had:

Repository

Both contained Git history.

That's Distributed Version Control.

Interview Questions
Q1. What are the types of Version Control Systems?

Answer

There are three types:

Local Version Control System
Centralized Version Control System
Distributed Version Control System

Git is a Distributed Version Control System.

Q2. Why is Git called a Distributed Version Control System?

Answer

Because every developer has a complete copy of the repository, including commit history, branches, and project files. Developers can continue working even if the remote server is temporarily unavailable.

Revision

Remember this simple evolution:

Local VCS

↓

Centralized VCS

↓

Distributed VCS (Git)
Practical Thinking Exercise (No Commands)

Imagine this scenario:

You are working on your Software-Engineer-Roadmap.
Your internet connection stops working for 2 hours.

Can you still:

Edit your Markdown files? ✅
Run git add .? ✅
Run git commit? ✅
View previous commits? ✅
Run git push? ❌ (No internet)

Why?

Because Git stores the repository locally in the hidden .git folder.

Homework

Create Types-of-Version-Control-System.md using the same documentation structure we've been following.