# Practical 1 — Git Installation, Configuration and GitHub Repository Setup

## 📌 Objective

To understand the fundamentals of Git by creating a local repository, tracking files, creating commits, connecting the local repository to a GitHub remote repository, and pushing the local changes to GitHub.

---

## 🎯 Learning Objectives

This practical demonstrates the following concepts:

* Creating directories and files using the command line
* Installing and verifying Git
* Initializing a local Git repository
* Checking repository status
* Staging files
* Creating commits
* Viewing commit history
* Creating and configuring a GitHub repository
* Adding a remote repository using `origin`
* Verifying the remote connection
* Renaming the default branch to `main`
* Pushing local commits to GitHub

---

## 🛠️ Tools Used

* Git
* Git Bash / Terminal
* Nano Text Editor
* GitHub

---

## 📂 Project Structure

The practical was created using the following structure:

```text id="s8h7tq"
PRACTICALS/
└── practical1/
    ├── README.md
    └── file1.txt
```

---

## 🔧 Practical Implementation

### 1. Create the Main Directory

Create the main directory for the DevOps practicals:

```bash id="0jap1u"
mkdir PRACTICALS
```

Navigate into the directory:

```bash id="l5v8t4"
cd PRACTICALS
```

---

### 2. Create the Practical Directory

Create a directory for Practical 1:

```bash id="h7k6zz"
mkdir practical1
cd practical1
```

---

### 3. Create a File

Create `file1.txt`:

```bash id="2ypfcz"
touch file1.txt
```

---

### 4. Edit the File

Open the file using Nano:

```bash id="gdj6ec"
nano file1.txt
```

Add the required content and save the file.

---

### 5. Display File Content

Verify the contents of the file:

```bash id="c5lqsh"
cat file1.txt
```

---

# 🌱 Local Git Repository

### 6. Initialize Git

Initialize a Git repository inside the `practical1` directory:

```bash id="xg6l3n"
git init
```

This creates a hidden `.git` directory that stores the repository's version-control information.

---

### 7. Check Repository Status

Check the current status of the repository:

```bash id="3g4k91"
git status
```

This displays information about the current branch and untracked or modified files.

---

### 8. Stage the Files

Add the files to the staging area:

```bash id="r5u1u2"
git add .
```

Verify the staging status:

```bash id="j6m2m3"
git status
```

The files should now appear under **Changes to be committed**.

---

### 9. Create the First Commit

Create a commit containing the staged changes:

```bash id="d0h8qx"
git commit -m "Initial commits"
```

The commit creates a snapshot of the staged files in the local Git repository.

---

## 📜 Git Commit History

### 10. View Commit History

View detailed information about previous commits:

```bash id="b2w0am"
git log
```

This displays information such as:

* Commit hash
* Author
* Date
* Commit message

---

### 11. View Compact Commit History

View the commit history in a concise format:

```bash id="8p4g6x"
git log --oneline
```

Example:

```text id="0x7y2z"
<commit-hash> Initial commits
```

---

# ☁️ GitHub Repository Setup

### 12. Create a GitHub Repository

A repository named **PRACTICALS** was created on GitHub.

The local repository was then connected to the GitHub repository.

---

### 13. Add GitHub as a Remote Repository

The GitHub repository was added as a remote using the conventional name `origin`:

```bash id="j3f8k9"
git remote add origin https://github.com/Sudhanshuraj1037/PRACTICALS.git
```

Here:

* `git remote add` — adds a remote repository
* `origin` — standard name assigned to the remote repository
* GitHub URL — address of the remote repository

---

### 14. Verify the Remote Repository

Verify that the remote repository has been configured correctly:

```bash id="q2m7vp"
git remote -v
```

Expected output:

```text id="x1a9bc"
origin  https://github.com/Sudhanshuraj1037/PRACTICALS.git (fetch)
origin  https://github.com/Sudhanshuraj1037/PRACTICALS.git (push)
```

---

### 15. Rename the Branch to `main`

The local branch was renamed from `master` to `main`:

```bash id="k7d3pz"
git branch -M main
```

The `main` branch is commonly used as the primary branch of a GitHub repository.

---

### 16. Push Local Repository to GitHub

Push the local `main` branch to the GitHub repository:

```bash id="a8r4nf"
git push -u origin main
```

The `-u` option establishes an upstream relationship between the local `main` branch and the remote `origin/main` branch.

After this, future pushes can generally be performed using:

```bash id="v4s2we"
git push
```

---

## 🔄 Complete Git Workflow

The complete workflow demonstrated in this practical is:

```text id="6q9r2t"
Create Directory
      │
      ▼
Create File
      │
      ▼
git init
      │
      ▼
git status
      │
      ▼
git add .
      │
      ▼
git commit
      │
      ▼
git log
      │
      ▼
Create GitHub Repository
      │
      ▼
git remote add origin
      │
      ▼
git remote -v
      │
      ▼
git branch -M main
      │
      ▼
git push -u origin main
      │
      ▼
     GitHub
```

---

## 📋 Commands Used

| Command                   | Purpose                                  |
| ------------------------- | ---------------------------------------- |
| `mkdir PRACTICALS`        | Creates the main practical directory     |
| `cd PRACTICALS`           | Navigates into the directory             |
| `mkdir practical1`        | Creates the Practical 1 directory        |
| `cd practical1`           | Navigates into the practical directory   |
| `touch file1.txt`         | Creates a new file                       |
| `nano file1.txt`          | Opens the file for editing               |
| `cat file1.txt`           | Displays file contents                   |
| `git init`                | Initializes a local Git repository       |
| `git status`              | Displays repository status               |
| `git add .`               | Stages all changes                       |
| `git commit -m`           | Creates a commit                         |
| `git log`                 | Displays detailed commit history         |
| `git log --oneline`       | Displays compact commit history          |
| `git remote add origin`   | Connects the local repository to GitHub  |
| `git remote -v`           | Displays configured remote repositories  |
| `git branch -M main`      | Renames the current branch to `main`     |
| `git push -u origin main` | Pushes the local `main` branch to GitHub |

---

## 🔑 Important Git Concepts

### Working Directory

The location where project files are created and modified.

### Staging Area

The intermediate area where changes are selected before committing.

### Local Repository

The Git repository stored on the local computer containing commits and project history.

### Remote Repository

The repository hosted on GitHub that allows code to be stored remotely and shared with others.

### `origin`

The conventional name given to the primary remote repository.

### `main`

The primary branch used in the repository.

---

## 🔄 Git Architecture

```text id="1s4k9m"
Working Directory
       │
       │ git add
       ▼
Staging Area
       │
       │ git commit
       ▼
Local Repository
       │
       │ git push
       ▼
Remote Repository
     (GitHub)
```

---

## ✅ Result

A local Git repository was successfully created and initialized. Files were created, staged, committed, and the commit history was inspected. The local repository was then connected to a GitHub remote repository using `origin`, and the `main` branch was successfully pushed to GitHub.

---

## 💡 Key Takeaway

This practical demonstrates the complete basic Git workflow from **creating a local repository to publishing it on GitHub**:

**Create → Track → Stage → Commit → Connect → Push**

This workflow forms the foundation for more advanced DevOps practices such as branching, merging, collaboration, containerization, and CI/CD automation.
