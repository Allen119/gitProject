# 🧠 Git Branching Strategy Project

This project demonstrates a real-world Git branching strategy commonly used in software teams to manage features, testing, hotfixes, and production releases. It builds on the fundamentals of Git and GitHub, and simulates how developers collaborate using branches, merges, rebases, and tags.

---

## 📁 Branches Overview

| Branch       | Purpose                                                                 |
|--------------|-------------------------------------------------------------------------|
| `featureX`   | Short-lived branches for specific features (e.g., `feature/login`)      |
| `integration`| Combines completed features for testing and staging                     |
| `hotfix`     | For urgent fixes that need to bypass the normal release cycle           |
| `production` | Stable code that is deployed to end users or live environments          |

---

## 🔁 Branching Workflow

1. ✅ Developers create **feature branches** from `integration`.
2. 🔄 Feature branches are **rebased or merged** into the `integration` branch after development.
3. 🧪 The `integration` branch is tested and then merged into `hotfix`.
4. 🚀 After hotfix validation, it is merged into `production`.

This allows parallel development, safer testing, and reliable releases.

---

## 🏷️ Git Tags

Tags are used to mark stable release points in the repository.

| Tag          | Meaning                                |
|--------------|----------------------------------------|
| `REL01.00.00`| First successful feature release        |
| `R02.00.00`  | Merged tested code into `hotfix` branch |
| `R02.00.01`  | Final stable release to production      |

Use tags to roll back or reference production-ready code easily.

---

## 📚 Key Git Concepts Practiced

- `git branch`, `git checkout`, `git switch`
- `git rebase`, `git merge`, `git reset`, `git stash`
- `git tag` (lightweight and annotated)
- Resolving merge conflicts
- Clean collaboration workflows
- Using `git log`, `git status`, and `git reflog` for navigation and recovery

---

## ✅ Example Diagram (as per strategy)

