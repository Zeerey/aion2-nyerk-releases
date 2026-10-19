# Troubleshooting

[← Back to Nyerk](../README.md)

## The download does not contain the application

Use the **Portable ZIP** under the release's **Assets**. GitHub's **Source code** ZIP is a copy of this documentation repository. Extract the complete portable ZIP before launching.

## Launch Nyerk.cmd cannot find the file

Keep the launcher beside **Aion2Nyerk.exe**, extract all files, and try opening the executable directly. Confirm that you are launching the intended folder rather than an older copy.

If Windows Security removed or blocked the file, follow the Windows security guidance below instead of repeatedly downloading or renaming it.

## Missing Npcap

Install Npcap from [npcap.com](https://npcap.com/#download), then restart Nyerk or choose **Start tracking** on Network. Npcap is required for live capture and is not bundled or silently installed by Nyerk.

## The interface is blank or does not open

Verify that you are using Windows 10/11 x64 and that the [WebView2 Runtime](https://developer.microsoft.com/en-us/microsoft-edge/webview2) is installed. Record the Nyerk version and any exact error for a bug report.

## Waiting for character identification

Start Nyerk before logging into the game. Check Network for capture status and dropped/discarded observations. Supported login messages give stronger identity evidence than joining a session after it is already underway.

Saved characters can still be displayed while current identity is unresolved. Pet collection is account-wide; a missing active character should not by itself prevent supported pet pickups from being tracked.

## Player names show “Actor,” or damage seems wrong

Nyerk needs supported identity and summon-owner messages as well as damage messages. Starting mid-dungeon can miss earlier evidence. Combat also remains experimental.

A useful comparison uses the **same completed encounter**, the **same target scope**, and both meters' **total damage, DPS and duration**. A brief peak during combat is not a final encounter average. State whether summons, multiple enemies or a mid-fight startup were involved. See [Support](../SUPPORT.md).

## A boss timer is wrong or missing

Check the selected character/server, map, channel and the timer's source/status. A scheduled estimate can drift when respawn depends on a kill. RC31 reads supported map lists and restores saved deadlines. Keep tracking enabled, identify your active character/server, then open Map → Exploration → Field monsters on the relevant map. Restored observations are not fresh checks. Abyss and other additional maps still need live acceptance, and channels are not decoded.

Report the game's countdown, Nyerk's countdown and the exact observation time with timezone. [Timer guide](TIMERS.md)

## The popout is missing or cannot be moved

Use **Ctrl + Alt + P** to show it. Use **Ctrl + Alt + L** to unlock it before dragging the title or pet strip. Check Settings → Popout to confirm the wanted modules are enabled.

An idle DPS area can be expected: unrelated nearby combat should not create your encounter. If the overlay unexpectedly prevents interaction with other apps, use Alt+Tab to regain focus and report the version and action that triggered it.

## The update icon does not glow

Current builds check at startup and every hour. Open the update panel for a manual check or any reported error. No glow can mean the installed build is already the newest eligible release.

Local development builds may be newer than GitHub. The updater will not downgrade them. A check does not install an update automatically.

## Windows reports a threat or blocks the updater

Keep Windows security intelligence current and note the exact detection name, Nyerk version and affected filename. Report those details without attaching private recordings. Do not disable protection or add an exclusion just to run Nyerk.

Unsigned-publisher warnings and malware detections are different. A clean scan or a previous Microsoft review does not guarantee that a different build will receive no warning. [Privacy and security details](PRIVACY_AND_SAFETY.md)

## Still stuck?

Use **Report a bug** in Nyerk or [open a bug report](https://github.com/Zeerey/aion2-nyerk-releases/issues/new?template=bug_report.yml). Include your version, Windows version, steps and expected/actual result.
