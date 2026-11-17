# My Tasks: releases

This repository holds only the built Mac app of **My Tasks** and the update file `latest.json` that the app reads for "Check for updates".
The source code is in a private repository.

## Install
1. Open the latest release and download `My Tasks_<version>_aarch64.dmg` (Apple Silicon).
2. Open the disk image and drag **My Tasks** to Applications.
3. The app is not signed with an Apple Developer ID. At the first start, right-click the app and select **Open**.

## Updates
The app checks this repository for a new version. Each update is signed with the app's update key, and the app refuses an update with a wrong signature.
