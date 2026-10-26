# Ardiment · current feature reference

Documented release: **0.7.1.1**, private beta. This describes the current application release, not the historical source snapshot included in the public repository.

## Established product decisions

| Decision | Current behavior |
| --- | --- |
| Final name | Ardiment; the name stays English in both interface languages. |
| Familiar visual character | Refined nested prism emblem, cyan/violet palette, dark and light modes. |
| One shared workspace | Full control, Guided, and Autopilot operate on the same records. Full control is the current default. |
| Recommendations use real work | Local eligibility/ranking can surface an actual task or unfinished step without a generative request. |
| Project work has a home | Project containers stay in Projects. Explicit task planning/deadlines can admit eligible work into daily recommendations. |
| Compact task presentation | Real next step and Start first; additional steps/details expand on demand. |
| Calendar lives with Quests | List and calendar are views of the same work; planned date and deadline remain distinct. |
| Completion earns rewards | Starting a timer, organizing work, routine check-ins, and social coordination do not automatically award personal quest XP. |
| One-task Complete all | Finishes the selected task and its remaining steps; protects prior rewards and availability constraints. |
| Habits/routines remain integrated | Life Systems supports routines, measures, manual records, reviews, and explicit links. |
| Privacy and recovery together | Settings provides distinct guidance for sign-in, cloud recovery, local protection, and backups. |
| Simplified destinations | Standalone Guide and Milestones are retired; assistance/history remain in current workspaces. |
| One appearance entry point | Theme & colors remains; redundant Advanced layout disclosure removed in 0.7.1.1. |

## Capability matrix

| Capability | Implemented scope | Dependency or limit |
| --- | --- | --- |
| Manual capture | Tasks, scheduling, steps, editing, and drafts. | Available without external semantic AI. |
| AI assistance | Submitted-text analysis and reviewed project/task proposals. | Configured server/provider and consent; local deterministic fallback has less semantic depth. |
| Study | Courses, semesters, timetable, study context, and linked work. | Academic context is not automatic proof of task completion. |
| Focus | Real step reference, optional timing, parked thoughts, session continuation. | Timing/parked notes are device-local. |
| Daily recurrence | Dated occurrences, retained history, constrained reversal. | Future occurrences remain locked until their date. |
| Projects | Required/optional work and gated final objectives. | Complete all does not bypass final gates. |
| Progress | Task XP, levels, ranks, transferable skills, titles/history. | App indicators, not professional credentials. |
| Local saving | Account/Guest-scoped persistence and pending sync state. | Device/browser storage availability matters. |
| Cloud progress | Browser-encrypted account state and guarded reconciliation. | Configured Supabase project, auth, and correct database policies. |
| Optional Privacy lock | Encrypted browser storage and inactivity/manual locking. | Separate local credentials; cannot defend an already compromised unlocked app. |
| Backups | Plain or password-protected portable copies. | Encrypted export password must be retained by the user. |
| Request portal | Encrypted proposed work, accepted only after review. | Server/database/anti-abuse setup required. |
| Friends/Circles | Optional shared coordination and contribution scopes. | Authorized service/database setup; not the private progress vault. |
| Notifications | Per-device foreground handling; optional background Web Push. | Background delivery needs subscriptions, VAPID/server configuration, authenticated scheduling, permission, and supported devices. |
| Offline shell | Cached resources and accessible saved work. | First cloud restore, auth, AI, and other server operations need connectivity. |
| Installation | PWA manifest/icons and platform installation guidance. | Browser/platform support and real-device acceptance; icon refresh timing varies. |
| English/Arabic | Localized UI, RTL, stable device language choice. | Authored text stays unchanged. |

Implementation and verification are different claims. See [verification](VERIFICATION.md) and [known issues](KNOWN-ISSUES.md).
