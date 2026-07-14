# THE GIT ARCHITECTURE

                    Git Architecture

        ┌─────────────────────────────┐
        │      Working Directory       │
        └─────────────────────────────┘
                     │
                     │ git add
                     ▼
        ┌─────────────────────────────┐
        │        Staging Area         │
        └─────────────────────────────┘
                     │
                     │ git commit
                     ▼
        ┌─────────────────────────────┐
        │      Local Repository       │
        │        (.git folder)        │
        └─────────────────────────────┘
                     │
                     │ git push
                     ▼
        ┌─────────────────────────────┐
        │     Remote Repository       │
        │    (GitHub/Azure DevOps)    │
        └─────────────────────────────┘

VS Code

↓

Ctrl + S

↓

Working Directory

↓

git add

↓

Staging Area

↓

git commit

↓

Local Repository (.git)

↓

git push

↓

GitHub
