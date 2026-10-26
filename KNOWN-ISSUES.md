# Ardiment · known issues and validation queue

Current documented application: **0.7.1.1**. Listed validation work is not a promise of a release date.

## UI-001 · Login security widget overlaps its copy

**Status:** open; recorded for a later update.  
**Reported platforms:** iPad and desktop.  
**Observed:** Cloudflare Turnstile's success/checkmark/logo box overlaps the Bot protection / Security check text in the login panel.  
**Scope:** layout/readability. A visible success label alone does not establish completion of account authentication.

### Acceptance criteria

- Give the security copy, widget, and status their own layout space.
- Prevent overlap at desktop/tablet widths, shorter windows, enlarged text, and narrow layouts.
- Check English/Arabic, both directions, light/dark, and widget loading/success/error states.
- Keep actual verification callbacks and protection behavior intact.

The private user screenshot is not included in this public kit. This issue was not fixed in 0.7.1.1.

## Acceptance work still required

| Area | Required check |
| --- | --- |
| Installation | Real iPhone/iPad name/icon refresh and installed-app behavior. |
| Offline upgrade | Real HTTPS shell update with existing tasks/preferences and pending edits retained. |
| Account continuity | Correct-account login and recovery on the new origin, then actual cross-device reconciliation. |
| Notifications | Supported Home Screen app, per-device permission, configured scheduler, and delivery with the app closed. |
| Access/layout | Full viewport blocking and responsive flow on real devices/browser zoom. |
| Broader assurance | Accessibility review, device performance measurement, and independent security review. |
