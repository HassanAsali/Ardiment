# Ardiment · passwords, files, and recovery

## Different credentials do different jobs

| Item | Purpose | Important limit |
| --- | --- | --- |
| Account password | Sign in to the Supabase-backed account. | A password reset does not recreate a lost encryption key. |
| Cloud Recovery File | Unlock the account's encrypted synced progress on a new browser/origin/device. | Holds a key, not a dated copy of tasks. |
| Local privacy password | Unlock this browser when optional Privacy lock is enabled. | Separate from account sign-in. |
| Local Recovery File | Recover that browser's local Privacy lock. | Bound to that local vault; not a cloud-unlock replacement. |
| Backup file | Portable copy of work/progress/settings for supported restoration. | Does not automatically include every device-local draft/session. |
| Encrypted-backup password | Decrypt a password-protected exported backup. | Must be retained; the app cannot recover a forgotten export password. |

## Existing recovery files after the rebrand

The Cloud Recovery Key still uses the **`ASCEND1.` prefix** for compatibility. Do not rename the prefix to Ardiment. An older file may still unlock current synced data if it belongs to the same account vault and the key has not changed.

Import the Cloud Recovery File through the app's file control, or paste only its complete recovery-key line. Do not paste the file title, email, version labels, or surrounding explanation into the key field.

### “Recovery key is invalid.”

The current parser decodes the supplied key and expects 32 bytes. This message indicates invalid key length at that parsing stage; it is not proof that a dated file is too old or that the account disappeared. A properly shaped key that cannot open the account vault has a separate mismatch/error path.

Check that the selected file is the Cloud Recovery File and that the pasted line is complete. Keep the key private. Do not post the file, key, or a revealing screenshot to GitHub or a public support thread.

## After changing the application domain

A new origin has separate browser storage. You can authenticate successfully and still need the Cloud Recovery File before reading encrypted progress. Once unlocked, only data that actually reached the cloud can be restored from that cloud copy.

Keep the original device/app and storage until the new-origin restoration is confirmed. If the key is unavailable but another trusted device still opens the account, export the Cloud Recovery File from that trusted app. If all keys and usable backups are lost, encrypted progress may be unrecoverable even with a valid sign-in password.

Guest work and unsynced changes need an accessible original-device backup/export. They are not contained in the Cloud Recovery File.
