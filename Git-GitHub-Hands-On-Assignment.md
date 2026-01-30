## New to Git & GitHub? Below assignment covers all the required basics to be confident as a DevOps Engineer.

![Git & GitHub](https://imgur.com/9yYHc6T.png)

---

## Skills

Below skills are required to complete this assignment:

Git basics, Git workflow, Branching & Merging, Conflict Resolution, GitHub collaboration, Rollback & Recovery

---

## Pre-Requisites

1. Install Git on your local machine
2. Create a GitHub account
3. Configure Git with username and email
4. Configure SSH key with GitHub
5. Create a working directory on your system

---

## Deployment

### 1. Local Git Setup (Repository Initialization)

1. Create a directory named `devops-git-lab`
2. Initialize Git repository inside it
3. Check Git status
4. Create files:
   - README.md
   - app.txt
5. Add files to staging area
6. Commit changes with message:  
   **"Initial commit – project setup"**

---

### 2. Branching & Feature Development

1. Create a new branch named `feature-login`
2. Switch to `feature-login` branch
3. Add below text to `app.txt`:
   ```
   Login feature under development
   ```
4. Commit changes with proper message
5. Switch back to `main` branch
6. Verify `app.txt` does NOT contain login feature

---

### 3. Merge Feature Branch

1. Merge `feature-login` branch into `main`
2. Verify merge is successful
3. View Git log and confirm merge commit
4. Delete `feature-login` branch

---

### 4. GitHub Integration

1. Create a **public repository** on GitHub named `devops-git-lab`
2. Add GitHub remote to local repository
3. Push `main` branch to GitHub
4. Verify files are visible on GitHub UI

---

### 5. Pull Request (PR) Workflow

1. Create a new branch `feature-logging`
2. Add below text to `app.txt`:
   ```
   Logging feature added
   ```
3. Commit changes
4. Push branch to GitHub
5. Create a Pull Request (PR) from `feature-logging` → `main`
6. Review PR and merge it
7. Delete feature branch after merge

---

### 6. Conflict Resolution (Critical DevOps Skill)

1. Create branch `conflict-branch`
2. Modify `app.txt` with:
   ```
   This line is from conflict branch
   ```
3. Commit changes
4. Switch to `main` branch
5. Modify the SAME line differently
6. Commit changes
7. Merge `conflict-branch` into `main`
8. Resolve merge conflict manually
9. Complete merge successfully

---

### 7. Rollback & Recovery (Production Simulation)

1. Create a bad commit by deleting `app.txt`
2. Commit the change
3. Realize mistake and rollback using:
   - git revert OR git reset
4. Restore `app.txt`
5. Verify file content is recovered

---

### 8. Git Stash (Real DevOps Scenario)

1. Modify `README.md` without committing
2. Stash changes
3. Verify working directory is clean
4. Apply stash and restore changes

---

### 9. Git Inspection & Auditing

1. View commit history
2. Identify author of each commit
3. Show difference between two commits
4. Find when a specific line was added

---

### 10. Cleanup & Best Practices

1. Delete all unused branches
2. Ensure `main` branch is clean
3. Add `.gitignore` file
4. Ignore:
   - *.log
   - *.tmp
   - node_modules/
5. Commit `.gitignore`

---

## Final Challenge (MANDATORY)

Simulate a **real DevOps incident**:

- A wrong change is merged into `main`
- Production is broken
- Identify faulty commit
- Roll back safely
- Document:
  - What went wrong
  - How it was fixed
  - How it can be prevented

---

## Outcome

After completing this assignment, you should be confident in:

- Daily Git usage
- Branching strategies
- Pull request workflow
- Conflict handling
- Rollback & recovery
- GitHub collaboration

---

All done? Still not confident?  
👉 **Repeat the steps until commands feel natural.**

**Happy Learning 🚀**
