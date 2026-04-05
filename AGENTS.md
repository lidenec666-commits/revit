# Revit Workspace Agent Rules

## Scope
- Treat this repository as a control point for local Windows work on this machine.
- When a task mentions local files, prefer explicit absolute Windows paths over virtual or read-only sources when the tools allow it.

## Local Paths
- If the user names folders like `Desktop`, `Documents`, `Downloads`, `REVIT`, `WORK`, or `ARCH`, inspect those locations directly before asking follow-up questions.
- Edit text-based local files by absolute path whenever possible.
- For binary files such as `.rvt`, `.rte`, `.dwg`, `.rar`, `.mp4`, `.jpg`, or `.pdf`, do not claim to rewrite internal content as text. Offer file operations around them instead: inspect, move, rename, copy, inventory, report, or automation.

## Automation
- Reuse the local toolkit in `C:\Users\Лидия\Desktop\CopilotSafeAutomation` when it matches the request.
- Prefer the `.cmd` launchers in that toolkit if PowerShell script execution is blocked.

## Repo Sync
- Treat `C:\Users\Лидия\Desktop\revit-github` as the canonical writable clone of `https://github.com/lidenec666-commits/revit`.
- When a task mentions `revit`, GitHub sync, pull, push, commit, or repository changes, inspect the local clone before using any virtual GitHub view.
- Before editing repo files or publishing changes, check repo state with `git status --short --branch` and refresh remote state with `git fetch origin`.
- If the local clone is clean and behind `origin/main`, prefer `git pull --ff-only origin main`.
- If the clone has local changes or diverged history, do not overwrite them during sync. Report the state and continue carefully.
- After changing repo instructions or other repo files, commit and push when the user asks to sync or publish.

## Limits
- Work within the tools and permissions actually available in the session.
- Do not claim unrestricted or hidden control over the machine.