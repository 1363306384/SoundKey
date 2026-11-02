# Install SoundKey

**English** · [简体中文](installation.zh-CN.md) · [Back to home](../README.md)

Download installers from the [1.0.0 release](https://github.com/1363306384/SoundKey/releases/tag/v1.0.0). The release includes a SHA-256 checksum file so you can verify your download.

| Platform | Download | Requirements |
| --- | --- | --- |
| Mac | `SoundKey-1.0.0-Mac-arm64.dmg` | Apple Silicon, macOS 13 or later |
| Windows | `SoundKey-1.0.0-windows-x64-Setup.exe` | Windows 10 or 11, x64 |

## Mac

The current Mac app uses an Apple Development signature. Its Installer package is unsigned, and the release is **not notarized by Apple**. macOS may require manual approval. This is not an App Store or Developer ID–notarized distribution.

1. Quit any running copy of SoundKey.
2. Open the downloaded DMG.
3. Run **安装SoundKey.command**. Read its notice, then type **INSTALL** to continue.
4. Complete the installation in Apple's Installer. It installs SoundKey in **Applications**.
5. Open **SoundKey** from Applications. A desktop Finder alias is created on first launch.

The command is the installation entry for this release. It verifies the adjacent `SoundKey.pkg` before preparing a temporary installation copy. Its quarantine repair is limited to that verified copy and the verified SoundKey app; it does not disable Gatekeeper globally. Do not separate it from its matching package or substitute a package from another release.

If Finder cannot run the command, open Terminal, type `/bin/bash` followed by a space, drag **安装SoundKey.command** from the mounted DMG into Terminal, and press Return. Read the notice and type **INSTALL** only if you intend to install this download. A checksum failure stops installation; download the matching release again rather than bypassing the check.

### Enable shortcuts in other apps

Music can be imported and played with the mouse before global shortcuts are set up.

1. Open SoundKey **Settings → Global Shortcuts → Open Input Monitoring**.
2. In **System Settings → Privacy & Security → Input Monitoring**, add or enable the SoundKey installed in Applications. SoundKey provides a drag bar for adding the app.
3. If macOS asks, choose **Quit & Reopen**. If SoundKey does not reopen, open it manually from Applications.
4. Return to SoundKey Settings and use **Check Again**. Keep **Music Shortcut Switch** enabled and close Settings before testing a bound key in another app.

A system switch being on does not always mean that the current process has picked up the grant. If SoundKey still reports that Input Monitoring is not active, quit SoundKey completely, reopen the Applications copy, and check again. Avoid running an older copy from a download folder or another disk image.

The package and permission recovery logic were checked locally. The first-authorization **Quit & Reopen** flow on another Mac running macOS 15.2 has not yet been verified.

## Windows

1. Quit SoundKey if it is running.
2. Run **SoundKey-1.0.0-windows-x64-Setup.exe**.
3. Follow the installer, then launch SoundKey from the desktop or Start menu shortcut.

The installer includes the required .NET runtime and import tools. It installs for the current user. The executable and installer are **not Authenticode-signed**, so Windows may show an unknown-publisher or SmartScreen notice. Check the download source and checksum before deciding whether to proceed.

Windows build, business-logic checks and package integrity checks passed. Native Windows installation, audio, interface and global-keyboard-hook testing remain outstanding.

## Update, backup and remove

Before updating, export a backup from **Library → Back Up and Restore Library**. Quit SoundKey, then install the newer package over the existing application. Keep your backup until you have checked the updated app.

The Windows uninstaller removes the application and shortcuts while retaining the local library. Removing the Mac application also leaves its separately stored library. Uninstalling is not a full data reset.

For everyday use, groups, shortcuts and backups, see the [user guide](user-guide.md).
