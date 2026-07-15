# Git Diff

## Definition

`git diff` is used to compare the differences between different Git areas. It shows the actual content (lines added, removed, or modified) instead of only displaying the file names.

---

## Syntax

```bash
git diff
```

```bash
git diff --staged
```

---

# git diff

## Purpose

Displays the differences between the **Working Directory** and the **Staging Area**.

It shows the changes that have been made but are **not yet staged**.

### Comparison

```text
Working Directory
        ↑
        │ git diff
        ↓
Staging Area
```

### Example

```bash
git diff
```

Output:

```diff
+ Line Added
- Line Removed
```

---

# git diff --staged

## Purpose

Displays the differences between the **Staging Area** and the **Local Repository (Last Commit)**.

It shows the changes that are already staged and will be included in the next commit.

### Comparison

```text
Staging Area
        ↑
        │ git diff --staged
        ↓
Local Repository (Last Commit)
```

---

# Difference between git diff and git diff --staged

| Command | Comparison | Purpose |
|----------|------------|---------|
| `git diff` | Working Directory ↔ Staging Area | Shows unstaged changes |
| `git diff --staged` | Staging Area ↔ Local Repository | Shows staged changes that will be committed |

---

# Common Scenario

Suppose:

```
Local Repository
Version 1

↓

Staging Area
Version 2

↓

Working Directory
Version 3
```

### git diff

Compares:

```
Working Directory (Version 3)

↓

Staging Area (Version 2)
```

Displays only the changes that are **not staged**.

---

### git diff --staged

Compares:

```
Staging Area (Version 2)

↓

Local Repository (Version 1)
```

Displays only the changes that are **already staged**.

---

# Interview Questions

### What is git diff?

`git diff` displays the content differences between the Working Directory and the Staging Area.

---

### What is git diff --staged?

`git diff --staged` displays the content differences between the Staging Area and the Local Repository (Last Commit).

---

### Key Points

- `git diff` shows unstaged changes.
- `git diff --staged` shows staged changes.
- Both commands display the actual modified content, not just the file names.
- `+` indicates an added line.
- `-` indicates a removed line.