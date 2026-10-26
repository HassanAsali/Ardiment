# ASCEND → Ardiment

## Final name and scope

**Ardiment** is the final product name. Use this spelling in ordinary interface and documentation text. **ARDIMENT** is reserved for intentional wordmark treatment. Keep the name English in Arabic interfaces. Do not attach an invented meaning, etymology, or pronunciation claim.

Version 0.7 evolved the existing 0.6.5.5.3 application. It did not create a new account system or replace the task model. Version 0.7.1.1 removes a duplicate appearance-settings disclosure.

## Updated surfaces

- Current interface, entry/onboarding copy, settings, public request page, notifications, recovery/backup filenames, titles, and metadata.
- Refined nested prism emblem, wordmarks, social artwork, vector sources, favicons, Apple touch artwork, PWA and maskable icons.
- Coordinated colors, shared components, compact tasks/menus/calendar tiles, responsive access gates, and completion feedback.
- One-task Complete all through the existing task, step, XP, and daily-recurrence rules.

No email templates or separate marketing landing page existed in the supplied application source. External provider sender names/templates and dashboard metadata still require owner review where configured.

## Compatibility-sensitive exceptions

| Retained identifier | Reason |
| --- | --- |
| `ascend.*` browser keys and IndexedDB names | Existing data and preferences must remain accessible. |
| `ASCEND1.` Cloud Recovery Key prefix | Previously exported keys must keep working. |
| Encryption format labels and AES-GCM associated data | Renaming authenticated identifiers can make existing ciphertext unreadable. |
| Backend tables/RPC names and auth metadata | Existing policies, integrations, and account state depend on them. |
| Package name, module globals, internal classes/file paths | Public branding does not require a breaking internal rename. |
| Manifest `id`, `start_url`, and `scope` of `/` | Preserve installed-app identity within the same origin. |
| Versioned `ascend-v…` cache family | Update the app shell without clearing user storage. |

Historical source/docs can still use ASCEND when describing that historical version. The repository URL can retain ASCEND until its owner chooses to rename it.

## Domain continuity is separate

The owner-provided current application URL is:

<https://ardiment-beta-nine.vercel.app>

Changing the hostname creates a separate browser-storage origin. Stable keys or a stable manifest path cannot transfer local storage across origins. A signed-in user may therefore need the existing Cloud Recovery File to unlock the encrypted cloud vault at the new address.

- Keep the original browser/app data until recovery and cloud restoration are confirmed.
- Guest-only work and unsynced changes require their own accessible backup or original-device export; a Cloud Recovery File contains no tasks.
- Preserve the same Supabase project and vault. A public rename does not require recreating accounts or backend tables.
- The owner must review Supabase site/redirect URLs, permitted Turnstile hostnames, and any existing request/callback links when changing domains.
- Existing push subscriptions and installed PWAs are origin-specific; a new origin may need installation/permission/subscription acceptance again. Preserve server VAPID keys rather than rotating them for branding.

No external configuration is changed by this showcase kit. [Recovery guide](RECOVERY.md) · [Brand reference](BRAND.md)
