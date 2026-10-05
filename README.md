# Google Drive Sync for Obsidian

Near-realtime vault sync through your own free Google Drive. Works on Windows, macOS, iOS and Android.

- Local edits push about 2 s after you stop typing.
- Remote changes are found via Drive's change feed (one tiny API call every 10 s), so it stays far below the free quota.
- Notes edited on two devices are merged line by line; binary conflicts keep both versions.
- Only files created by the plugin are visible to it (drive.file scope).

## Setup
1. Google Cloud Console: create a project, enable the Google Drive API, configure the OAuth consent screen and publish it to production.
2. Create an OAuth client of type "TVs and Limited Input devices" and copy the client ID and secret.
3. Install this plugin (BRAT: add beta plugin rabby0101/obsidian-gdrive-sync), paste the same client ID and secret on every device, set the same Drive folder name, and press Sign in.
