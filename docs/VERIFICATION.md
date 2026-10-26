# Ardiment · verification scope

Recorded evidence for the documented releases. No live CI badge or independent security certification is implied.

## 0.7.1.1

The full `npm test` command completed successfully. It contains **24 Node test suites** covering static/unit behavior, task/domain logic, sync reconciliation/resilience, server/security guards, account isolation, privacy cryptography, calendar behavior, service-worker handling, and mocked service paths.

The changed `experience-workspace.js` passed a JavaScript syntax check. Source review confirmed removal of the duplicate Advanced layout markup while preserving the Theme & colors action. The app version and cache build were updated.

No fresh browser/device or live-account acceptance pass was run for this small patch. Its UI screenshots remain the 0.7 fixture captures and are labeled accordingly.

## 0.7 automated checks

The regression suite passed. Added checks cover one-task Complete all with partial progress, one save/celebration, repeated activation, remaining reward totals, untouched unrelated records, locked project finals, future daily tasks, next-day recurrence, and stable manifest names/identity. Offline cache-alias checks cover versioned installation assets.

These are static/unit/mocked integration checks, not live-cloud proof. Historical test messages can retain their original version labels; suite counts are taken from the packaged test command rather than interpreted from those labels.

## 0.7 interface QA

Actual public app files ran in an isolated static fixture with synthetic Guest data and mocked disabled-cloud configuration. The HTTP fixture supplied a UUID fallback for that test context; production continued to require HTTPS/localhost and retained its security headers.

| Scenario | Recorded observation |
| --- | --- |
| English desktop, 1280px | Sampled dark-mode interface; no horizontal page overflow or broken images in inspected views. |
| Arabic tablet, 820px | RTL interface, task menu, and compact calendar inspected. |
| Arabic phone, 375px | Light-mode layout and wrapping inspected. |
| Restore gate, 820 × 500 | Gate matched viewport height; underlying app inert. |
| Action menu sample | Approximately 131 × 184px with 42px rows. |
| Several tasks on one calendar date | Approximately 70px per tile in the tablet sample. |
| Complete all via keyboard | Parent and remaining steps completed; synthetic XP changed from 1840 to 1885 for a 45 XP task. |

The final sampled fixture path had no new app runtime exception. An earlier HTTP-only UUID issue was isolated to the fixture. Production security headers blocked subresource execution on the managed HTTP preview, so that server path was not used to claim production browser acceptance.

## Not verified by these checks

- Real iPhone/iPad Safari installation, application-name/icon refresh, or physical-device rendering.
- Live Supabase authentication/policies, actual cross-device cloud restoration, and production offline upgrades.
- Actual notification permission/subscription/delivery or authenticated background scheduling.
- Live AI provider behavior, encrypted external-request delivery, or external dashboard changes.
- Production frame performance, exhaustive accessibility, or independent security review.

The subsequent user-reported Cloudflare widget overlap is explicitly [open](KNOWN-ISSUES.md); prior sampled QA is not evidence that this issue is fixed.

## Showcase validation

The documentation kit is checked separately for local links/images, SVG structure/rendering, current naming/version claims, image validity, and accidental inclusion of credentials or runtime account data. GitHub's own Markdown/Mermaid rendering still needs a preview after upload.
