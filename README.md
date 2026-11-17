# My Tasks: releases

This repository holds only the built Mac app of **My Tasks** and the update file `latest.json` that the app reads for "Check for updates".
The source code is in a private repository.

## Install
1. Open the latest release and download `My Tasks_<version>_aarch64.dmg` (Apple Silicon).
2. Open the disk image and drag **My Tasks** to Applications.
3. Open **My Tasks** from Applications. The app is not signed with an Apple Developer ID, so macOS says that it could not verify the app. Click **Done**, not Move to Trash.
4. Open **System Settings > Privacy & Security**. In the **Security** section, click **Open Anyway** next to the line about My Tasks. Confirm with your password or Touch ID, then click **Open Anyway** again.
   - Or, in Terminal: `xattr -dr com.apple.quarantine "/Applications/My Tasks.app"`
5. This is necessary one time only. Updates that the app installs itself do not show the message.

## Updates
The app checks this repository for a new version. Each update is signed with the app's update key, and the app refuses an update with a wrong signature.
