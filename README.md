# Trunk-Based Development

This repository demonstrates **Trunk-Based Development**.
This strategy is commonly used in modern CI/CD pipelines.

## About the Project
This is a static Library Dashboard built using:
- HTML
- CSS

---

## Branching Model

Trunk-Based Development uses **one main branch**.

### Trunk Branch
- **main**
  - The single source of truth
  - Always stable and deployable

### Short-Lived Branches
- **short/***
  - Created from `main`
  - Exist for a very short duration (hours or days)
  - Merged back into `main` quickly

---

## Branch Flow Diagram
```
short-lived branch → main
```

---

## Workflow
1. Create a short-lived branch from `main`
2. Make a small change
3. Merge back into `main as soon as possible
4. Delete the branch after merge

---

## Key Principles
- No long-lived branches
- Frequent commits and merges
- Strong CI required
- Feature flags preferred for incomplete features

---

## Purpose
- Minimize merge conflicts
- Enable rapid and safe deployments
- Encourage continuous integration

---

## Deployment
The `main` branch is always production-ready and deployable.
