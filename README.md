# Git Real-World Workflows – DevOps Practice Lab

## 📌 Overview
This repository demonstrates real-world Git workflows used by DevOps and engineering teams.
It focuses on safe collaboration, mistake recovery, and production rollbacks.

The goal of this lab is to practice how to work in team environments without breaking production.

---

## 🎯 Objectives
- Work safely using branching strategies
- Follow a proper Pull Request (PR) workflow
- Resolve merge conflicts confidently
- Recover from common Git disasters
- Perform safe rollbacks in production environments

---

## 🌿 Branching Strategy

main
 ├── dev
 │    ├── feature/login
 │    ├── feature/dashboard

### Branch Purpose
- main: Production-ready code
- dev: Integration branch
- feature/*: Individual feature development

Rules:
- No direct commits to main
- All changes go through dev
- Feature branches are merged using PRs

---

## 🔁 Pull Request (PR) Workflow
1. Create a feature branch from dev
2. Make changes and commit
3. Open a PR to merge into dev
4. Review and test changes
5. Merge dev into main for release

Why PRs matter:
- Code review
- CI checks before merge
- Prevents accidental production breaks

---

## ⚔️ Merge Conflict Resolution

Scenario:
Two branches modify the same file and same line.

Resolution:
1. Identify conflict markers
2. Decide correct changes
3. Remove conflict markers
4. Commit resolved version

Key learning:
Merge conflicts are normal in team environments.

---

## 🚨 Git Disaster Recovery Scenarios

### Scenario 1: Accidental Commit to main
Solution:
git revert <commit_id>

Why:
- Preserves history
- Safe for shared branches

---

### Scenario 2: Wrong Merge Happened
Solution:
git revert -m 1 <merge_commit_id>

---

### Scenario 3: Rollback Production Release
Solution:
git revert HEAD
or
git checkout <stable-tag>

Rule:
Never use git reset on shared branches.

---

## 🔧 Advanced Git Commands Used
- git stash
- git rebase
- git cherry-pick
- git revert

---

## ⚖️ Reset vs Revert

git reset:
- Rewrites history
- Dangerous on shared branches

git revert:
- Preserves history
- Safe on shared branches

---

## 🧠 Real DevOps Learnings
- Git is risk management
- Protect production branches
- Rollbacks should be safe and auditable

---

## 🏁 Conclusion
This repository demonstrates production-ready Git practices used in real DevOps teams.

Interview summary:
I follow PR-based Git workflows, handle merge conflicts, and perform safe production rollbacks.
