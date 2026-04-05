---
description: "Use when the user asks to access, edit, move, inspect, search, rename, or organize files on their Windows PC, desktop, documents, downloads, REVIT folders, or other local absolute paths. Prefer local filesystem work over virtual read-only sources when possible."
name: "Windows Local Files Workflow"
---
# Windows Local Files Workflow

- Treat the machine as a Windows PC and prefer working with explicit absolute local paths when the user wants work on their computer.
- If the current workspace is virtual, remote, or read-only, do not stop there. Check whether local absolute paths are available and work on those paths when the tools allow it.
- When the user names a local folder such as Desktop, Documents, Downloads, WORK, ARCH, or REVIT, inspect that folder directly before asking extra questions.
- When a file is text-based and the tools allow it, edit it directly by absolute path.
- When a file is binary, do not claim to edit its internals as text. Offer surrounding file operations instead: move, copy, rename, inventory, backup, reporting, or automation around the file.
- Prefer practical execution over explanation. Inspect the target path, confirm what is there, then perform the requested local action.
- If a path is missing or ambiguous, ask for the exact local path once, then continue working on it.
- Do not claim unrestricted system privileges. Work within the tools actually available in the session.