# CC AI BOT - full standalone office PC

## Download the current setup

- [Full Windows desktop setup 10.8.3](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/CCTech-AI-Bot-Setup-10.8.3.exe)
- [Android app 2.5](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/CC-AI-BOT-2.5.apk)
- [Installation manual (PDF)](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/CC-AI-BOT-Installation-and-User-Manual.pdf)
- [Office installation instructions (Notepad)](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/READ-ME-FULL-OFFICE-PC.txt)
- [Current release and integrity files](https://github.com/chandra15031993-dev/cctech-bot-updates/releases/tag/updates)

## Install on the office PC

Close the old Office Client, run **10.8.3** in its existing installation directory, then launch the **CC AI BOT desktop shortcut**. This installer always selects the full standalone Host, including upgrades from the limited Office Client. It runs the complete desktop terminal and OpenAlgo server on the office PC. The old/home PC does not need to remain online.

The full desktop interface includes Scanner, Positions & Orders, Markets, Market Pulse, AI Agents, Options, Research and Settings. Python, Tk and application dependencies are bundled for Windows 10/11 64-bit. Fresh accounts start in DEMO without broker credentials. Set up your own broker IDs and local OpenAlgo API key, and verify Analyzer before real-money use. Existing local data is preserved. Advanced setup and broker authorisation require your account configuration.

Android 2.5 includes dedicated Market Trend and AI Agent screens, sector breadth, price trends, candidate reasons and independent scan/entry controls. Pair it using a **new link from the office PC's Settings > Mobile app**. Private remote access requires that office host's companion/Tailscale configuration. The office PC runs the engine and must stay awake while trading. Phone lane startup supports confirmed Analyzer execution; LIVE startup and advanced AI provider/policy configuration remain on the desktop.

## Settings update address

```text
https://github.com/chandra15031993-dev/cctech-bot-updates/releases/download/updates/release.manifest
```

The new packages have this address preset. Older PC installations can save it in Settings > Help > Software updates & office setup; Android uses Settings > Updates. Check, download and confirm installation. PC upgrades require closing the desktop/client and stopping the verified idle owned server first. No update automatically starts trading.

The updater verifies the pinned RSA/SHA-256 manifest signature, artifact size and SHA-256. Android also requires its existing signing identity. The Windows installer has no Authenticode publisher certificate. Direct-download hashes are in SHA256SUMS.txt.

## Moving accounts and protecting data

The public packages contain application code and the desktop dock arrangement. They do not contain personal broker credentials, account databases, pairing vaults or private signing keys. Enter your own IDs on the office PC. Optional encrypted backup/restore is available separately for private history.

Cloud Drive/OneDrive/Dropbox folders are for backups, not a shared live database. Stop entries and review positions/orders on the old host before moving an account to the office PC. Re-pair Android with the office host.

## Future releases

Keep the existing update-signing and Android signing keys private. Build both artifacts, verify them, upload them to the stable **updates** release, then replace release.manifest last. Keep the stable feed address unchanged. Older versioned assets may remain for history; use the current versions linked above.
