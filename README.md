# CC AI BOT updates

Signed Windows and Android update downloads for CC AI BOT by CCTech IT Solutions. This repository distributes release packages; it does not contain personal trading databases, broker credentials, pairing vaults or private signing keys.

## Current release

Windows **10.8.1** / Android **2.4** (Android version code 15).

[Open downloads and release notes](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/tag/updates)

## Set up Settings updates once

Copy this exact address into the update settings of older installations:

```text
https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/release.manifest
```

- **PC:** Settings > Help > Software updates & office setup. Paste and save the address, check for updates, then download the verified installer. Close the host/client and use Stop idle host server for update before installing. Do not interrupt open trades or remove protective orders to force an update.
- **Android:** Settings > Updates > Check Android software updates. Paste the address if blank, check/download, then choose Install verified download. Install over the existing production app to preserve pairing. Android may ask for installation permission and confirmation.

The update address is preset in Windows 10.8.1 and Android 2.4. Future release packages must still be built, signed and published before Check for updates can discover them. Updates are not silently installed and do not start trading automatically.

## Direct installation

- [Windows installer 10.8.1](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/CCTech-AI-Bot-Setup-10.8.1.exe) — Windows 10/11 x64.
- [Android APK 2.4](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/CC-AI-BOT-2.4.apk) — Android 8 or newer.
- [SHA-256 checksums](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/SHA256SUMS.txt).

On an office PC, choose **Office client — shared existing host** and pair it with the existing trading host. Keep one active trading host for the account. Do not share a live SQLite database through a cloud-sync folder. The full installer includes its private Python runtime and dependencies; the office PC does not need developer SDKs.

## Verification

The updater verifies the pinned RSA/SHA-256 signature on release.manifest and then the package hash and size. Android also checks the installed package's signing identity. The Android signing identity is retained from 2.3. The Windows installer does not have a Windows Authenticode publisher certificate; signed update metadata is a separate verification mechanism.

## Changes in this release

Independent Scanner, Market Pulse and AI Agent discovery controls; source-labelled, expiring Almost Ready handoffs; all seven supported exchange choices; shared position, budget and entry-risk checks; preset signed update feed. An eligible signal is not a guarantee of profit.

## Publishing later versions

Preserve the existing private release-signing key and Android keystore outside this repository. Increment the Windows version and Android version code, rebuild and verify both packages, upload the new packages to the editable `updates` release, and replace the signed release.manifest last. Keep older packages available so cached manifests still resolve. Never publish credentials, databases or private signing material.
