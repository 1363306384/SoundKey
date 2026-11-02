# SoundKey user guide

**English** · [简体中文](user-guide.zh-CN.md) · [Back to home](../README.md)

SoundKey keeps music in groups and lets you start a track with a key or key combination. You can begin with mouse playback and set up shortcuts later.

## Your first track

1. Click **Import Local Music** and choose an audio file. MP3, M4A and WAV are good starting points; other formats depend on the platform's audio support.
2. Click a row to select it, then press the bottom **Play** button. The small play button beside a track starts it directly.
3. Click **Set Shortcut**, press your chosen key or combination, and save it.
4. Keep **Music Shortcut Switch** enabled. On Mac, complete [Input Monitoring setup](installation.md#enable-shortcuts-in-other-apps) to use the binding while another app is in front.

Imported audio is copied into the local library. Moving the original file afterward does not break that imported copy.

## Playback controls

| Control | Behavior |
| --- | --- |
| Bound key | Starts its assigned track or playback range in the active group |
| Space in the main window | Plays the selected track, or pauses/resumes current playback |
| Back/forward buttons | Move the playback position by five seconds |
| Stop | Ends current playback |
| Play Once / Repeat List / Repeat One | Choose what happens when the track or range finishes |
| Speed and volume | Adjust playback speed and master volume |

Click the playback-mode button to cycle through its three modes. Playback is limited to the range you set for that track, if any.

Shortcut capture, text editing and open dialogs can temporarily suspend music-key handling so your typing does not trigger a track. Close the dialog before testing playback keys. Pausing the music shortcut switch does not disable mouse playback.

## Organize groups

Use the group selector to choose the music available to your shortcuts. **Manage Groups** opens the group overview, where you can create, rename, switch between groups and remove empty groups. Group order is not editable. Different groups can reuse the same music shortcut; duplicate assignments within one group are rejected.

Drag a track's handle to reorder it. Open its **…** menu to edit its title/range, move it to another group, or move it to **Recently Deleted**. A move that would duplicate an existing shortcut in the destination is refused until the conflict is resolved.

## Play only a clip

Open **… → Title and Playback Range**. Enter a start and end time using seconds or `minutes:seconds`, for example `30` or `0:50`. **Use Current** takes the position from that track's current playback. Reset the range to return to full-track playback.

The range affects playback without trimming or replacing the stored audio file.

## YouTube and link import

The toolbar has separate **YouTube** and **Import Link** actions. **YouTube** opens **Search YouTube**, where you can search by song, artist or keyword. **Preview** opens the original YouTube page in your default browser; it does not add the result to your library. **Import** downloads one result to the group chosen when that import starts.

**Import Link** opens **Import from Link** for a single public HTTP(S) video-page or audio-file link supported by the bundled downloader. Imported downloads are converted to MP3. An internet connection is required, and availability depends on the source site.

Only one online import runs at a time. Search remains available while a download is running. You can close either online-import window and let the download continue, then reopen it from the toolbar or **View Progress**. Switching groups does not change a running import's destination. **Cancel Download** is available during downloading/conversion; the final save is completed as one operation and is not advertised as cancellable.

Sign-in, browser-cookie import, VIP access, paywalls and playlist importing are not supported by this workflow. A search result appearing is not a guarantee that its audio can be downloaded. Import only material you are permitted to use.

## Back up, restore and recover

On both platforms, the top **Library** menu contains **Back Up and Restore Library** and **Recently Deleted**. Open **Library → Back Up and Restore Library** to export a `.soundkeybackup` file. A backup contains all groups and their music, titles, order, playback ranges, shortcuts and playback settings. Store a copy somewhere outside the app's library folder.

**Restore from Backup replaces all active groups, tracks and playback settings** after confirmation. Export the current library first if you want to keep it. Backups can move a library between Mac and Windows; review any warning about a shortcut that cannot be mapped on the other platform.

For an accidentally removed track, open **Library → Recently Deleted → Restore**. It returns to its original group, or the current group if the original no longer exists. Resolve any shortcut conflict first; recovery does not overwrite another assignment. Recently Deleted is local recovery storage, so do not rely on it as your only backup.

## Language and local data

Open **Settings → Language** to switch between **English** and **中文** immediately. English is the default for a new installation. Language choice is saved for later use.

SoundKey stores its library and imported music locally. To move to another computer, use the backup/export flow rather than copying the application alone. Uninstalling the app does not automatically erase its separately stored library.

## If a shortcut does not play

1. Confirm the correct group and assigned key, and turn on **Music Shortcut Switch**.
2. Close shortcut capture, text fields and dialogs, then test in the main window.
3. On Mac, check **Settings → Global Shortcuts**. If Input Monitoring is enabled in macOS but not active for SoundKey, quit and reopen the Applications copy, then click **Check Again**.
4. Test in another app only after the global status is ready. Other apps and macOS may reserve particular key combinations; choose another binding if needed.

For installation and the scope of representative Windows checks, see the [installation guide](installation.md) and [release verification notes](releases/1.0.1.md#verification-scope).
