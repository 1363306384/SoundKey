<p align="center">
  <img src="docs/images/soundkey-banner.png" alt="SoundKey — Your music. One keystroke away." width="100%">
</p>

<p align="center">
  <strong>English</strong> · <a href="README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  A native music and sound cue player for macOS and Windows.<br>
  Build your library, assign a key, and keep your next cue within reach.
</p>

<p align="center">
  <a href="https://github.com/1363306384/SoundKey/releases/latest"><strong>Download SoundKey</strong></a> ·
  <a href="docs/user-guide.md">User guide</a> ·
  <a href="docs/installation.md">Installation</a> ·
  <a href="https://github.com/1363306384/SoundKey/issues">Feedback</a>
</p>

## Meet SoundKey

SoundKey keeps music, transitions, and short sound cues in a focused desktop library. Use it for live streams, rehearsals, presentations, or your own listening setup. Organize tracks into groups, set the part you want to play, and trigger a track with its assigned keyboard shortcut.

![SoundKey for macOS with a sample music library](docs/images/library-en.jpg)

*macOS interface with fictional sample tracks. Demo audio is not included in the download. Windows follows the same content layout and workflow, with native Windows text and window controls.*

## Download 1.0.3

| Platform | Requirements | Installer |
| --- | --- | --- |
| macOS | Apple Silicon · macOS 13 or later | [Download .dmg](https://github.com/1363306384/SoundKey/releases/download/v1.0.3/SoundKey-1.0.3-Mac-arm64.dmg) |
| Windows | Windows 10 or later · x64 | [Download Setup.exe](https://github.com/1363306384/SoundKey/releases/download/v1.0.3/SoundKey-1.0.3-windows-x64-Setup.exe) |

**Current signing status:** the Mac app has a development signature and is **not notarized**; the Windows installer is **unsigned**. Manual system approval may be required. See the [installation guide](docs/installation.md) before installing on another computer.

On Mac, open the disk image, run the included **Install SoundKey.command**, type **INSTALL**, and finish the macOS Installer. The helper is part of this release's installation flow; its purpose and the fallback steps are documented in the guide. Open the installed app from **Applications**.

On Windows, quit any running copy of SoundKey and run **Setup.exe**. Setup and uninstall are in English; the app itself supports English and Chinese.

[Release notes](docs/releases/1.0.3.md) · [SHA-256 checksums](https://github.com/1363306384/SoundKey/releases/download/v1.0.3/SHA256SUMS.txt)

## A small set of useful controls

| Feature | What you can do |
| --- | --- |
| Shortcut overview | Review group bindings and the keyboard diagram; edit, clear or locate a track from one place. |
| Keyboard cues | Assign keys to tracks, use a configurable Pause / Resume key (M by default), or pause all music shortcuts with one switch. |
| Groups | Keep different sets of tracks together, with each group's track order and shortcut assignments. |
| Local imports | Import supported audio files in the background, with progress, duplicate choices and batch cancellation. SoundKey saves a library copy. |
| Local MP4 to MP3 | Extract audio offline to a 192 kbps MP3, with a save location of your choice. |
| Playback ranges | Set a start and end point for a track without editing the original recording. |
| Playback controls | Seek, adjust master volume, choose a speed, and play once or repeat a track or list. |
| Online discovery | Search YouTube, preview the original page in your browser, or import a supported link. |
| Library recovery | Export and restore library backups, or recover tracks from Recently Deleted. |
| Two languages | Switch between English and 简体中文 in Settings. |

Online imports need an internet connection and depend on the source site's availability. Use content you have permission to download. Login, subscription, DRM-protected, and other restricted content are not supported.

## Your first cue

1. Choose **Import Local Music** and select an audio file.
2. Click a track to select it; double-click to play. Selecting a different track leaves the bottom player on the music that is actually playing. In the main window, **Space** plays your selection or pauses/resumes the current track.
3. Choose **Set Shortcut** on a track and record the key you want to use.
4. For shortcuts while using another app on Mac, open **Settings → Global Shortcuts** and complete **Input Monitoring** setup. Quit and reopen SoundKey if macOS requests it.

Music still plays with the mouse when music shortcuts are paused. The app distinguishes in-window shortcuts from global access; the system's permission switch alone does not confirm that the running listener is ready.

## English or Chinese

The app starts in English. Open **Settings → Language → 中文** to switch immediately. To read these docs in Chinese, choose **简体中文** at the top of any guide.

![SoundKey language and shortcut settings](docs/images/settings-en.jpg)

## Help and feedback

Start with the [user guide](docs/user-guide.md) and [installation troubleshooting](docs/installation.md). If you still need help, [open an issue](https://github.com/1363306384/SoundKey/issues/new/choose) with your OS version, chip/architecture, SoundKey version, and steps to reproduce. English and Chinese reports are welcome. Remove personal information from screenshots and logs before posting.

SoundKey 1.0.3 adds a shortcut overview with a fixed keyboard diagram, binding edits and track location on both platforms. Click to select, double-click to play; the bottom player follows actual playback independently of selection. It also fixes missing-file removal and Windows shortcut priority. See the [release notes](docs/releases/1.0.3.md) for validation scope. Native Windows testing and another Mac's first Input Monitoring grant/relaunch flow remain unverified.

## About this repository

This repository contains product documentation, images, and downloadable releases. **SoundKey application source code is not published here.** Third-party components keep their respective licenses; see [Third-party notices](docs/third-party-notices.md).
