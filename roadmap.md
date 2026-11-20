# Claude Control feature roadmap
2026-11-20
## Roadmap
Claude Control already shows every Claude Code conversation on the machine in one VS Code list, marks a status as a guess when it cannot confirm it, and shows how old its usage figures are. Next come a more direct live signal from Claude Code's own session list, Open VSX and Windows support, and tidying conversations from the row menu.
| Feature | Priority | Status | Sources | Notes |
| --- | --- | --- | --- | --- |
| **Knowing which conversation needs you** |  |  |  |  |
| See every conversation that is waiting for you at the top of the list | High | Done | Claude Code agent view, Claude Control Panel, Claude Code GitHub issues | Waiting conversations are pinned to the top. |
| See how many conversations are waiting from the status bar, with the sidebar closed | High | Done | Claude Code agent view, Claude Control Panel | A bell shows "N waiting" and opens those conversations. |
| Know when a filter is hiding a waiting conversation | High | Done | Claude Code GitHub issues | A notice offers to show all. |
| Tell a confirmed wait from a likely one | High | Done | Claude Control Panel | An unconfirmed wait shows as "Waiting?" with a faded icon. |
| Get a notification when a conversation starts waiting | Medium | Done | Claude Code agent view, Happy, Claude Code GitHub issues | Optional, once per change, with an Open button. |
| See waiting status sooner, from Claude Code's own list of running sessions | High | Partly done | Claude Control Panel, Claude Code agent view | Already used as one of four signals; to become the first one. |
| Skip the notification when you are already looking at that conversation | Medium | To do | Hacker News | |
| **Usage limits** |  |  |  |  |
| See session, weekly and model limits as bars at the foot of the list | High | Done | Claude Code /usage, Claude Code Usage History, Claude Code Manager, Claude Control Panel | The limit currently in force is bold. |
| See how old the usage figures are | High | Done | Claude Code GitHub issues | "as of 8h ago", fading after 15 minutes. |
| See the next reset in plain words | High | Done | Claude Code GitHub issues | For example "Resets 2am tomorrow". |
| Get an early colour warning before a limit | Medium | Done | Hacker News | Orange from 75%, red from 90%. |
| Read usage from Claude Code's status line data | High | To do | Claude Code Manager | Avoids running a separate Claude command to refresh. |
| **The conversation list** |  |  |  |  |
| See panel and terminal conversations from every project in one list | High | Done | Claude Code Manager, Claude Control Panel, Claude Code Sessions | Filter by project, state or search. |
| See each conversation's permission mode, with bypass in red | Medium | Done | Claude Code GitHub issues | Uses Claude Code's own icons and labels. |
| See the model each conversation uses | Low | Done | | OPUS, SONNET, HAIKU, FABLE. |
| Delete, rename or archive a conversation from its row | Medium | To do | Claude Code Sessions, Claude Code Manager, Claude Code GitHub issues | |
| See worktree conversations grouped with their repository | Medium | To do | Claude Code agent view, Claude Code GitHub issues | |
| Search the full text of every transcript | Low | To do | Claude Code Usage History, Claude Code Manager | Today search covers title, prompt, project, branch and status. |
| See a conversation's subagents | Low | To do | Claude Control Panel | |
| Reach the row menu by keyboard and hear status changes with a screen reader | Medium | To do | | Rows already open with Enter or Space. |
| **Continuing on another device** |  |  |  |  |
| Hand a conversation to the Claude mobile app from its row | Medium | Partly done | Claude Code Remote Control, Happy, Claude Code GitHub issues | Live conversations still need Enter pressed once. |
| Start Remote Control for a whole folder from the title bar | Medium | Done | Claude Code Remote Control | Asks first, checks folder trust, stops only what it started. |
| **Changed files** |  |  |  |  |
| See the files a finished run changed and open a Before and After diff | Medium | Done | VS Code sessions view, Claude Code Usage History, Claude Squad | Scratch files and deleted files are left out. |
| See a count when a run changed more than 40 files | Low | To do | | |
| **Platforms and setup** |  |  |  |  |
| Install from Open VSX in Cursor and other editors | High | To do | Claude Control Panel, Claude Code | |
| Use it on Windows | Medium | To do | Claude Control Panel, Claude Code | Tested on Linux so far. |
| Turn precise status on and off without touching your own hooks | Medium | Done | Claude Control Panel | Settings are backed up first and restored exactly. |
| Follow the editor's colour theme everywhere | Low | Partly done | | The project dropdown does not follow it yet. |
## Session tools for Claude Code compared
**Claude Code (VS Code extension, agent view, Remote Control).** Anthropic's own tools. The VS Code extension has a session history with status filters per workspace, a usage dialog, and Remote Control. Agent view lists background sessions across projects in the terminal. Included with a paid Claude plan.

**VS Code sessions view.** Built into VS Code. Lists agent sessions from several harnesses, including Claude Code, with a summary of changes. Free.

**Claude Control Panel.** A VS Code and Cursor extension that shows live sessions with subagents, waiting alerts, usage gauges and configuration editing. Free and open source.

**Claude Code Manager.** A VS Code extension for sessions, usage limits, accounts, MCP servers and hooks. Free and open source.

**Claude Code Usage History.** A VS Code extension for browsing and searching history across several coding agents, with diffs and quota. Free with a paid tier.

**Claude Code Sessions.** A VS Code extension that shows projects and sessions as a tree, with resume, rename, delete and move. Free.

**Claude Squad.** A terminal app built on tmux that runs several coding agents with preview and diff views. Free and open source.

**Happy.** Mobile and desktop apps for following and driving coding agents, with push notifications. Free and open source.

**Hacker News and Claude Code GitHub issues.** Forums where Claude Code users describe these needs; counted as request sources, not products.
