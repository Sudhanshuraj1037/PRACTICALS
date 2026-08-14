# Practical 2 — Git Basic Commands

## 📌 Objective

To understand and practice the basic Git commands used to monitor, track, modify, stage, and manage files in a local Git repository.

---

## 🎯 Learning Objectives

This practical demonstrates the following Git concepts:

* Checking the repository status
* Creating and modifying files
* Tracking changes
* Staging files
* Viewing differences between changes
* Committing changes
* Viewing commit history
* Understanding the Git working directory and staging area

---

## 🛠️ Tools Used

* Git
* Git Bash / Terminal
* Text Editor

---

## 📂 Project Structure

```text
PRACTICALS/
└── practical2/
    ├── README.md
    └── file2.txt
```

---

## 🔧 Practical Implementation

### 1. Check Repository Status

The current state of the Git repository can be checked using:

```bash
git status
```

This command displays information about:

* Current branch
* Modified files
* Untracked files
* Staged changes
* Uncommitted changes

---

### 2. Create a New File

A new file can be created using:

```bash
touch file2.txt
```

The file can then be edited using a text editor.

---

### 3. Check File Status

After creating or modifying a file, check the repository status:

```bash
git status
```

Git identifies files that are not yet being tracked by the repository.

---

### 4. Add Files to the Staging Area

To stage a specific file:

```bash
git add file2.txt
```

To stage all changes:

```bash
git add .
```

The staging area allows specific changes to be selected before creating a commit.

---

### 5. Verify Staged Changes

After staging files, verify their status:

```bash
git status
```

The staged files will appear under:

```text
Changes to be committed
```

---

### 6. View Changes

The `git diff` command is used to view changes that have been made but are not yet staged:

```bash
git diff
```

To view changes that are already staged:

```bash
git diff --staged
```

These commands help verify changes before committing them.

---

### 7. Commit Changes

After reviewing and staging the changes, create a commit:

```bash
git commit -m "Update practical2"
```

A commit creates a permanent snapshot of the staged changes.

---

### 8. View Commit History

The complete commit history can be viewed using:

```bash
git log
```

For a compact history:

```bash
git log --oneline
```

---

## 🔄 Basic Git Workflow

The practical demonstrates the following workflow:

```text
Working Directory
       │
       │  Modify / Create Files
       ▼
    git status
       │
       ▼
     git add
       │
       ▼
 Staging Area
       │
       ▼
    git diff --staged
       │
       ▼
   git commit
       │
       ▼
   Repository
       │
       ▼
    git log
```

---

## 📋 Commands Used

| Command             | Purpose                                |
| ------------------- | -------------------------------------- |
| `git status`        | Displays the current repository status |
| `touch file2.txt`   | Creates a new file                     |
| `git add file2.txt` | Stages a specific file                 |
| `git add .`         | Stages all changes                     |
| `git diff`          | Displays unstaged changes              |
| `git diff --staged` | Displays staged changes                |
| `git commit -m`     | Creates a commit                       |
| `git log`           | Displays detailed commit history       |
| `git log --oneline` | Displays compact commit history        |

---

## ✅ Result

The basic Git commands were successfully practiced to monitor repository status, track files, stage changes, inspect differences, create commits, and view the commit history.

---

## 💡 Key Takeaway

Git provides a structured workflow for managing changes:

**Working Directory → Staging Area → Local Repository**

Understanding this workflow is essential before moving on to GitHub repository management, branching, merging, collaboration, and CI/CD practices.
