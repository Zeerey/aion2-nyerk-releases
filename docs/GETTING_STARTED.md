# Getting started with Nyerk

[← Back to Nyerk](../README.md)

## Requirements

| Requirement | Details |
| --- | --- |
| Operating system | Windows 10 or Windows 11, 64-bit |
| Game traffic | [Npcap](https://npcap.com/#download) |
| Desktop interface | [Microsoft Edge WebView2 Runtime](https://developer.microsoft.com/en-us/microsoft-edge/webview2) |
| Internet access | Downloads, update checks and enabled online features |

macOS and Linux builds are not currently available.

## First launch

1. Open the [recommended public release](https://github.com/Zeerey/aion2-nyerk-releases/releases/tag/v1.0.0-rc.28).
2. Under **Assets**, download **Aion2Nyerk-1.0.0-rc.28-Portable.zip**.
3. Extract the whole ZIP into a folder you can write to. Do not run it from inside the archive.
4. Install Npcap from its official website if needed, then run **Launch Nyerk.cmd** or **Aion2Nyerk.exe**.
5. Start tracking if it is stopped, then log into AION 2. Starting Nyerk before login gives it the best opportunity to observe your character identity.
6. Open **Settings → Popout** to choose the modules and timer alerts you want.

An initial **Searching for AION2.exe**, waiting or identification message is not itself a failure. The game must be running, capture must be available, and relevant data must arrive. If the status does not progress, use the [troubleshooting guide](TROUBLESHOOTING.md).

## Which download do I need?

| Asset | Purpose |
| --- | --- |
| **Aion2Nyerk-…-Portable.zip** | Recommended first download. Includes the app, launcher, instructions and third-party notices. |
| **Aion2Nyerk-Windows-x64.exe** | Application executable used by the built-in updater. |
| **SHA256SUMS.txt** | Checksums for verifying the downloaded files. |
| **Source code (zip / tar.gz)** | GitHub-generated copy of this documentation repository. It does not contain the Nyerk application. |

The public RC builds are marked as prereleases. GitHub's automatic **Latest** link may therefore point to an older build. Use the recommended download on the [front page](../README.md#download).

## Updating

Nyerk checks at startup and every hour. A download icon in the header and companion popout glows when a newer compatible version is available.

1. Open the update panel and review the available version.
2. Choose **Download update**.
3. Finish your encounter or diagnostic recording.
4. Choose **Install & restart**.

The popout download icon opens the main application's update panel. Checks alone do not download or restart anything. RC2 and later support the updater; hourly checking was introduced in RC9. You can check manually from the update panel.

For a manual update, close Nyerk normally, extract the new portable ZIP, and launch that copy. Keep one obvious installation folder to avoid accidentally opening an older copy.

## Your data

Profiles, settings and recordings are stored in:

```text
%APPDATA%\Aion2Nyerk
```

Updating the executable preserves this data. Before moving computers or making manual data changes, close Nyerk and back up that folder. Do not publish its contents in a GitHub issue.

## Popout basics

| Action | Shortcut / control |
| --- | --- |
| Show or hide the popout | Ctrl + Alt + P |
| Lock or unlock the popout | Ctrl + Alt + L |
| Move it | Unlock it, then drag its title or pet strip |
| Choose Pets, Combat and Timers | Settings → Popout |
| Choose event reminders | Timer alert selections in popout settings |
| Adjust appearance | Popout opacity and layout controls |

The DPS portion grows as contributors appear. Nearby combat alone should not open your encounter. An unresolved name means Nyerk has not received enough supported identity information to name that source.

[Need help?](../SUPPORT.md)
