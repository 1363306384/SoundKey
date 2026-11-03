# SoundKey user guide

**English** · [简体中文](user-guide.zh-CN.md) · [Back to home](../README.md)

SoundKey keeps music in groups and lets you start a track with a key or key combination. You can begin with mouse playback and set up shortcuts later. Mac and Windows use the same content layout, action order and dialog flows; window controls, file pickers, key names and global-shortcut permission setup are native to each platform.

## Your first track

1. Click **Import Local Music** and choose an audio file. MP3, M4A and WAV are good starting points; other formats depend on the platform's audio support.
2. Click a row to select it; double-click to play. The bottom player keeps showing and controlling the most recently played track independently of selection. The small play button beside a track starts it directly.
3. Click **Set Shortcut**, press your chosen key or combination, and save it.
4. Keep **Music Shortcut Switch** enabled. On Mac, complete [Input Monitoring setup](installation.md#enable-shortcuts-in-other-apps) to use the binding while another app is in front.

Imported audio is copied into the local library. Moving the original file afterward does not break that imported copy.

Batch imports check and copy files in the background. Follow progress while continuing playback, search, volume adjustment or group switching; new music still goes into the group selected at the start. Cancel Import withdraws the whole batch before the final save. Editing, deleting, backup and restore wait until the import finishes. For duplicates, skip, import anyway, view the existing track, or cancel the batch.

## Playback controls

| Control | Behavior |
| --- | --- |
| Bound key | Starts its assigned track or playback range in the active group |
| Pause / Resume shortcut (M by default) | Pause or resume the current track; change or clear it in Settings → Shortcuts |
| Space in the main window | Plays the selected track, or pauses/resumes current playback |
| Back/forward buttons | Move the playback position by five seconds |
| Stop | Ends current playback |
| Play Once / Repeat List / Repeat One | Choose what happens when the track or range finishes |
| Speed and volume | Adjust playback speed and master volume |

The pause shortcut does not start playback from idle. If a track already uses M, its binding is kept on upgrade; choose another pause shortcut. Pause and track shortcuts must be different across all groups.

Click the playback-mode button to cycle through its three modes. Playback is limited to the range you set for that track, if any.

Shortcut capture, text editing and open dialogs can temporarily suspend music-key handling so your typing does not trigger a track. Close the dialog before testing playback keys. Pausing the music shortcut switch does not disable mouse playback.

## Shortcut overview

Open **Library → Shortcut Overview** to review the selected group's track bindings and the global Pause / Resume shortcut. Edit or clear a binding, or choose **Locate** to return to the main list.

The overview's group picker only changes what you browse. Editing another group's shortcuts keeps the active group and playback. Locate switches the main library group and follows the existing group-switch playback behavior.

The full keyboard stays fixed above a fixed table header. Only the binding list scrolls.

The keyboard shows assigned keys in blue and unassigned keys in gray for the selected modifiers. The Mac diagram follows a compact ANSI Apple keyboard, including a wide space bar, Fn / Globe, modifiers and arrow keys. Click its Control, Option, Shift or Command keys to inspect combinations. Windows uses modifier checkboxes. Fn / Globe and Touch ID are shown as system keys and cannot be assigned on their own. Hover to see a track name, click an assigned key to edit or clear it, or click an unassigned key to choose a track or the pause action. Bindings outside the schematic keyboard remain visible in the list. Music shortcuts are suspended while the overview is open; closing it preserves the original master switch state.

Occupancy reflects SoundKey assignments only. It does not detect or guarantee availability in other apps or the operating system.

## Organize groups

Use the group selector to choose the music available to your shortcuts. **Manage Groups** opens the group overview, where you can create, rename, switch between groups and remove empty groups. Rename a group directly in the overview with Save or Cancel. Group order is not editable. Different groups can reuse the same music shortcut; duplicate assignments within one group are rejected.

Drag a track's handle to reorder it. Open its **…** menu to edit its title/range, move it to another group, or move it to **Recently Deleted**. A move that would duplicate an existing shortcut in the destination is refused until the conflict is resolved.

## Play only a clip

Open **… → Title and Playback Range**. Enter a start and end time using seconds or `minutes:seconds`, for example `30` or `0:50`. **Use Current** takes the position from that track's current playback. Choose **Use Full Track** to return to full-track playback.

The range affects playback without trimming or replacing the stored audio file.

## Convert a local MP4 to MP3

On Mac and Windows, open **Library → Local MP4 to MP3**, choose one local `.mp4` file, then choose where to save the `.mp3`. Click **Convert** to extract the first audio track as a 192 kbps MP3. This works offline and preserves the original MP4. Videos without an audio track cannot be converted.

The conversion window shows progress and lets you cancel while converting. Closing it during conversion cancels the task; the final save finishes as one operation. An existing destination file is replaced only after you approve the save dialog's overwrite prompt and conversion succeeds. Failed or cancelled conversions remove their temporary output and preserve any existing destination file.

After success, use **Show in Finder** on Mac or **Open Save Location** on Windows to locate the MP3. To use it in SoundKey, choose **Import Local Music** and select the saved MP3.

## YouTube and link import

The toolbar has separate **YouTube** and **Import Link** actions. **YouTube** opens **Search YouTube**, where you can search by song, artist or keyword. **Preview** opens the original YouTube page in your default browser; it does not add the result to your library. **Import** downloads one result to the group chosen when that import starts.

**Import Link** opens **Import from a Link** for a single public HTTP(S) video-page or audio-file link supported by the bundled downloader. Imported downloads are converted to MP3. An internet connection is required, and availability depends on the source site.

Closing Search YouTube cancels an active search and retains the latest query/results for reopening. Only one online import runs at a time. Search remains available while a download is running. You can close either online-import window and let the download continue, then reopen it from the toolbar or **View Progress**. Switching groups does not change a running import's destination. **Cancel Download** is available during downloading/conversion; the final save is completed as one operation and is not advertised as cancellable.

Sign-in, browser-cookie import, VIP access, paywalls and playlist importing are not supported by this workflow. A search result appearing is not a guarantee that its audio can be downloaded. Import only material you are permitted to use.

## Back up, restore and recover

On both platforms, the top **Library** menu contains **Back Up and Restore Library** and **Recently Deleted**. Open **Library → Back Up and Restore Library** to export a `.soundkeybackup` file. A backup contains all groups and their music, titles, order, playback ranges, shortcuts and playback settings. Store a copy somewhere outside the app's library folder.

**Restore from Backup replaces all active groups, tracks and playback settings** after confirmation. Export the current library first if you want to keep it. Backups can move a library between Mac and Windows; review any warning about a shortcut that cannot be mapped on the other platform.

Moving a track to Recently Deleted asks for confirmation; **Undo** in the notice can restore it immediately. For an accidentally removed track, open **Library → Recently Deleted → Restore**. It returns to its original group, or the current group if the original no longer exists. Resolve any shortcut conflict first; recovery does not overwrite another assignment. Recently Deleted is local recovery storage, so do not rely on it as your only backup.

## Language and local data

Open **Settings → Language** to switch between **English** and **中文** immediately. English is the default for a new installation. Language choice is saved for later use.

SoundKey stores its library and imported music locally. To move to another computer, use the backup/export flow rather than copying the application alone. Uninstalling the app does not automatically erase its separately stored library.

## If a shortcut does not play

1. Confirm the correct group and assigned key, and turn on **Music Shortcut Switch**.
2. Close shortcut capture, text fields and dialogs, then test in the main window.
3. On Mac, check **Settings → Global Shortcuts**. If Input Monitoring is enabled in macOS but not active for SoundKey, quit and reopen the Applications copy, then click **Check Again**.
4. Test in another app only after the global status is ready. Other apps and macOS may reserve particular key combinations; choose another binding if needed.

For installation and the current verification scope, see the [installation guide](installation.md) and [release verification notes](releases/1.0.2.md#verification-scope).
