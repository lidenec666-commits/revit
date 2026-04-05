---
description: "Use when the user asks to sync, synchronize, pull, push, commit, publish, or keep the revit GitHub repository up to date between VS Code and https://github.com/lidenec666-commits/revit."
name: "Revit Git Sync Workflow"
---
# Revit Git Sync Workflow

- Use `C:\Users\Лидия\Desktop\revit-github` as the writable local clone for repository sync tasks.
- If the user is looking at a virtual GitHub folder, prefer the local clone for inspection, edits, commits, and push operations.
- Start sync work by checking `git status --short --branch` and `git fetch origin`.
- If the working tree is clean and only needs updates from GitHub, use `git pull --ff-only origin main`.
- Never overwrite local uncommitted changes during sync.
- After repo edits, commit and push when the user asks to sync, publish, or save the changes to GitHub.