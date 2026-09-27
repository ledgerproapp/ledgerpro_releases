# LedgerPro

Encrypted receivables and payables tracking that works offline.

## Download

**[Download the latest version](https://github.com/ledgerproapp/ledgerpro_releases/releases/latest)** and pick the file for your computer:

| System | File |
|---|---|
| Windows 10/11 (Intel / AMD, 64-bit) | `LedgerPro-vX.Y.Z-win-x64.zip` |
| Windows 11 ARM (Snapdragon, Surface) | `LedgerPro-vX.Y.Z-win-arm64.zip` |
| macOS 12+ Apple Silicon (M1–M4) | `LedgerPro-vX.Y.Z-mac-arm64.zip` |
| macOS 12+ Intel | `LedgerPro-vX.Y.Z-mac-x64.zip` |
| Linux 64-bit | `LedgerPro-vX.Y.Z-linux-x64.AppImage` |

No installation is needed. The app checks for a new version when it starts and keeps working normally without internet. Data is stored encrypted in the `data` folder next to the app.

**Windows:** Extract the ZIP to a folder or a USB drive and run `LedgerPro.exe`.

**macOS:** Open the ZIP and move `LedgerPro.app` to a folder or a USB drive.
1. The app is not signed, so before the first start run this command once in Terminal. The path must be the folder where you put LedgerPro:

   ```
   xattr -dr com.apple.quarantine /Volumes/USB/LedgerPro
   ```

2. If macOS asks for Keychain access, choose **Always Allow**. Because the app is unsigned, this may be asked once more after each update. If you choose **Deny**, the app cannot open, but no data is lost; open it again and allow access.

**Linux:** Put the `.AppImage` file in a folder and make it executable:

```
chmod +x LedgerPro-*.AppImage
```

- GNOME Keyring or KWallet is required. Some distributions also need the `libfuse2` package.
- On Ubuntu 24.04 and later, AppArmor may block the sandbox of AppImage apps. If the app does not open, start it from a terminal with `./LedgerPro-*.AppImage --no-sandbox`. This setting is kept when the app restarts after an update.

This repository is for end-user distribution only; it does not contain source code.
