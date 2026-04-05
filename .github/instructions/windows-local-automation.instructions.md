---
description: "Use when the user asks to automate their Windows PC, open folders, open URLs, start programs, search local files, inspect processes, or generate a quick local system report. Includes the desktop toolkit in CopilotSafeAutomation."
name: "Windows Local Automation Toolkit"
---
# Windows Local Automation Toolkit

- Reuse the local toolkit in `C:\Users\Лидия\Desktop\CopilotSafeAutomation` when it matches the user's request.
- For interactive local actions, prefer `C:\Users\Лидия\Desktop\CopilotSafeAutomation\Launch-Control-Center.cmd`.
- For direct commands, prefer `C:\Users\Лидия\Desktop\CopilotSafeAutomation\Run-Action.cmd` with actions such as `system-info`, `open-folder`, `open-url`, `start-path`, `find-file`, `processes`, and `report`.
- If PowerShell script execution is blocked, use the provided `.cmd` wrappers rather than asking the user to weaken the global execution policy.
- For local PC tasks, default to transparent, user-visible actions and inspect existing scripts before creating new ones.
- If the user wants work in a specific folder, inspect that local path first and then decide whether the toolkit is needed.