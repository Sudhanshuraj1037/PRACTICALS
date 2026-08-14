# 🚀 DevOps Practicals — Semester 5

A structured collection of **DevOps practicals, experiments, configurations, and hands-on implementations** completed as part of the **5th Semester DevOps curriculum**.

This repository documents my practical journey from **Git and GitHub fundamentals** to **Docker containerization and Jenkins CI/CD pipelines**, with an emphasis on understanding the tools through hands-on implementation.

> 🎯 **Goal:** Build a strong practical foundation in modern DevOps practices, version control, containerization, automation, and Continuous Integration/Continuous Delivery (CI/CD).

---

## 📚 Practical Roadmap

The practicals covered in this repository are organized progressively, starting with version control and moving toward CI/CD automation.

| #  | Practical                             | Key Concepts                                                  |
| -- | ------------------------------------- | ------------------------------------------------------------- |
| 01 | Installation and Configuration of Git | Git installation, configuration, identity setup               |
| 02 | Git Basic Commands                    | `init`, `add`, `commit`, `status`, `log`, `diff`, etc.        |
| 03 | GitHub Repository Management          | Remote repositories, push, pull, clone, repository management |
| 04 | Branching & Merge                     | Branch creation, switching, merging                           |
| 05 | Conflict Resolution                   | Merge conflicts, conflict resolution, commit history          |
| 06 | GitHub Collaboration                  | Remote collaboration, pull requests, team workflows           |
| 07 | Rebasing, Tagging & Stashing          | Rebase, tags, stash, history management                       |
| 08 | Docker Installation                   | Docker setup and configuration                                |
| 09 | Dockerfile & Container Management     | Images, containers, Dockerfiles, build and run operations     |
| 10 | Jenkins Installation & Freestyle Job  | Jenkins setup and freestyle project configuration             |
| 11 | Jenkins Declarative Pipeline          | Pipeline-as-Code, Jenkinsfile, CI/CD automation               |

---

## 🧭 Learning Progression

The practicals follow a progressive DevOps workflow:

```text
Git
 │
 ▼
GitHub
 │
 ▼
Branching & Collaboration
 │
 ▼
Conflict Resolution
 │
 ▼
Advanced Git
 │
 ▼
Docker
 │
 ▼
Containerization
 │
 ▼
Jenkins
 │
 ▼
CI/CD Pipeline
```

The objective is not only to execute commands, but to understand **how these tools fit together in a real-world DevOps workflow**.

---

## 🛠️ Technologies & Tools

The repository primarily focuses on the following technologies:

| Technology                  | Purpose                                    |
| --------------------------- | ------------------------------------------ |
| 🐙 Git                      | Distributed Version Control                |
| 🐙 GitHub                   | Remote Repository & Collaboration          |
| 🐳 Docker                   | Containerization                           |
| 🔨 Jenkins                  | CI/CD Automation                           |
| 💻 Linux / Windows Terminal | Command-Line Operations                    |
| 📦 Git Bash                 | Git and Unix-like command-line environment |

---

## 📂 Repository Structure

The repository is organized according to the practical sessions:

```text
PRACTICALS/
│
├── practical1/
│   └── file1.txt
│
├── practical2/
│   └── ...
│
├── practical3/
│   └── ...
│
├── practical4/
│   └── ...
│
├── practical5/
│   └── ...
│
├── practical6/
│   └── ...
│
├── practical7/
│   └── ...
│
├── practical8/
│   └── ...
│
├── practical9/
│   └── ...
│
├── practical10/
│   └── ...
│
├── practical11/
│   └── ...
│
└── README.md
```

Each practical will contain the relevant **commands, configuration files, source files, screenshots, notes, and implementation details** where applicable.

---

## 📋 Practical Details

### 01 — Installation and Configuration of Git

**Topics covered:**

* Installing Git
* Configuring username and email
* Verifying Git installation
* Understanding Git configuration
* Initializing a repository
* Connecting local repositories with remote repositories

**Key commands:**

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --list
git init
```

---

### 02 — Git Basic Commands

**Topics covered:**

* Repository initialization
* Working directory
* Staging area
* Commits
* Viewing repository status
* Viewing commit history
* Comparing changes

**Key commands:**

```bash
git init
git status
git add .
git commit -m "Commit message"
git log
git diff
```

---

### 03 — GitHub Repository Management

**Topics covered:**

* Creating GitHub repositories
* Connecting local and remote repositories
* Cloning repositories
* Pushing changes
* Pulling changes
* Managing remote repositories

**Key commands:**

```bash
git clone <repository-url>
git remote -v
git remote add origin <repository-url>
git push -u origin main
git pull origin main
```

---

### 04 — Branching & Merge

**Topics covered:**

* Creating branches
* Switching branches
* Feature branches
* Merging branches
* Understanding branch workflows

**Key commands:**

```bash
git branch
git branch feature-name
git switch feature-name
git merge feature-name
```

---

### 05 — Conflict Resolution

**Topics covered:**

* Understanding merge conflicts
* Identifying conflicting files
* Resolving conflicts manually
* Staging resolved files
* Completing merge operations

Typical workflow:

```bash
git pull
# Resolve conflicts
git add .
git commit
```

---

### 06 — GitHub Collaboration

**Topics covered:**

* Collaborative Git workflows
* Pull Requests
* Code review
* Forking repositories
* Working with remote branches
* Synchronizing changes

The practical demonstrates how GitHub enables multiple developers to work on the same project.

---

### 07 — Rebasing, Tagging & Stashing

**Topics covered:**

* Git rebase
* Interactive rebase
* Creating tags
* Listing tags
* Temporary storage using stash
* Applying and removing stashed changes

**Key commands:**

```bash
git rebase main
git tag v1.0
git tag
git stash
git stash list
git stash pop
```

---

### 08 — Docker Installation

**Topics covered:**

* Installing Docker
* Verifying Docker installation
* Understanding Docker architecture
* Docker CLI
* Docker Engine
* Running the first container

**Key commands:**

```bash
docker --version
docker info
docker run hello-world
```

---

### 09 — Dockerfile & Container Management

**Topics covered:**

* Docker images
* Containers
* Dockerfiles
* Building images
* Running containers
* Starting and stopping containers
* Removing containers and images
* Port mapping

**Key commands:**

```bash
docker build -t myapp .
docker images
docker run -d -p 8080:8080 myapp
docker ps
docker stop <container-id>
docker rm <container-id>
```

---

### 10 — Jenkins Installation & Freestyle Job

**Topics covered:**

* Jenkins installation
* Jenkins configuration
* Creating Freestyle projects
* Build configuration
* Source Code Management
* Build triggers
* Build execution
* Build history

The practical introduces Jenkins as an automation server and demonstrates the fundamentals of CI.

---

### 11 — Jenkins Declarative Pipeline

**Topics covered:**

* Pipeline fundamentals
* Jenkinsfile
* Declarative Pipeline syntax
* Stages and steps
* Automated builds
* Pipeline execution
* CI/CD concepts

Example pipeline structure:

```groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
```

---

## 🔄 DevOps Workflow

The concepts covered in this repository can be combined into a simplified DevOps workflow:

```text
        ┌───────────────┐
        │   Developer   │
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │      Git      │
        │ Version Control│
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │    GitHub     │
        │ Collaboration │
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │    Jenkins    │
        │ CI/CD Pipeline│
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │    Docker     │
        │ Containerize  │
        └───────────────┘
```

This workflow demonstrates the relationship between **version control, collaboration, automation, and containerization**.

---

## 🎯 Learning Objectives

By completing these practicals, the following skills are developed:

* Understanding distributed version control with Git
* Managing repositories using GitHub
* Working with branches and merges
* Resolving merge conflicts
* Collaborating through GitHub
* Understanding advanced Git operations
* Creating and managing Docker containers
* Building Docker images using Dockerfiles
* Configuring Jenkins
* Creating Jenkins Freestyle projects
* Writing Jenkins Declarative Pipelines
* Understanding fundamental CI/CD workflows
* Applying DevOps concepts through hands-on practice

---

## 📈 Progress Tracker

| Practical | Topic                             | Status |
| --------- | --------------------------------- | :----: |
| 01        | Git Installation & Configuration  |    ✅   |
| 02        | Git Basic Commands                |    ⬜   |
| 03        | GitHub Repository Management      |    ⬜   |
| 04        | Branching & Merge                 |    ⬜   |
| 05        | Conflict Resolution               |    ⬜   |
| 06        | GitHub Collaboration              |    ⬜   |
| 07        | Rebasing, Tagging & Stashing      |    ⬜   |
| 08        | Docker Installation               |    ⬜   |
| 09        | Dockerfile & Container Management |    ⬜   |
| 10        | Jenkins Freestyle Job             |    ⬜   |
| 11        | Jenkins Declarative Pipeline      |    ⬜   |

> **Legend:** ✅ Completed · 🚧 In Progress · ⬜ Pending

---

## 🧪 Approach

Each practical is intended to follow a consistent hands-on approach:

```text
Understand
    ↓
Configure
    ↓
Implement
    ↓
Test
    ↓
Document
    ↓
Verify
```

Where appropriate, practical folders will include:

* Command references
* Configuration files
* Source code
* Dockerfiles
* Jenkinsfiles
* Screenshots
* Execution results
* Notes and observations

---

## 📖 References

The practical work is based on concepts and workflows from the official documentation of the respective technologies:

* Git Documentation
* GitHub Documentation
* Docker Documentation
* Jenkins Documentation

---

## 👨‍💻 About This Repository

This repository is maintained as part of my **5th Semester DevOps coursework** and serves as a practical record of my learning journey.

Rather than treating the practicals as isolated exercises, this repository is intended to demonstrate the progression from **fundamental version control concepts to automated CI/CD workflows**.

---

## ⭐ Future Scope

As my DevOps learning progresses, this repository may be extended with additional topics such as:

* Docker Compose
* Jenkins + Docker integration
* CI/CD with GitHub
* Linux administration
* Shell scripting
* Infrastructure as Code
* Terraform
* Kubernetes
* Cloud platforms
* Monitoring and observability
* Advanced CI/CD workflows

---

## 📌 Repository

**GitHub:**
[Sudhanshuraj1037/PRACTICALS](https://github.com/Sudhanshuraj1037/PRACTICALS?utm_source=chatgpt.com)

---

> **Learning by building. ♥️ Automating by understanding. ❤️**
