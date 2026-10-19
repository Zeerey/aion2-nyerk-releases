# Privacy and Windows security

[← Back to Nyerk](../README.md)

## How Nyerk observes the game

Nyerk uses Npcap to read supported game traffic locally. It does not inject into or modify AION 2, and it does not require your game password. Only supported observations can populate the interface; unavailable information can remain unknown.

This describes how the application works. It is not an endorsement by the game publisher or a guarantee about publisher policies.

## Local data and optional recordings

Characters, preferences, collection information and recordings are stored under:

```text
%APPDATA%\Aion2Nyerk
```

Public release downloads do not contain developer captures or user profiles. Diagnostic packet recording is a tool for investigating a particular problem. Raw recordings can include sensitive game and network information; do not attach them to public issues.

The in-app bug-report summary deliberately excludes character names, local file paths, recording notes and packet contents. You review the summary before opening GitHub, then submit the report yourself. Anything you add to a public issue, including screenshots, is public.

## Online connections

Nyerk is not completely offline. Online features can contact:

- GitHub to check release information and download an update you request.
- Public profile/image services for supported character and pet imagery.
- Configured timer sources when those features are enabled.
- GitHub or Ko-fi in your browser when you choose reporting or donation links.

The application does not automatically attach raw diagnostic recordings to a bug report. Review content before sharing it, and keep passwords, tokens and private captures out of public issues.

## What Microsoft's review means

The developer submitted an executable after an incorrect detection was reported. Microsoft's response stated that its scanners showed no positive detection and that it had no associated telemetry indicators for the submitted file.

That result applies to the submitted executable. It is **not Microsoft certification**, a code-signing certificate, an approval of the project as a whole, or a guarantee for future builds. Updating the application changes the file being assessed.

## Signing and download integrity

Current release candidates are unsigned. Windows can therefore show an unknown-publisher or reputation warning even when a scan finds no threats.

Release assets include **SHA256SUMS.txt**. Checksums help confirm that the downloaded bytes match the published files; they do not prove software safety or identify a trusted publisher. The in-app updater checks its downloaded file against GitHub's reported digest.

If Windows reports a threat, keep protection enabled and report the detection name, version and file involved. Do not bypass it by adding exclusions or renaming the executable.

[Installation](GETTING_STARTED.md) · [Troubleshooting](TROUBLESHOOTING.md) · [Support](../SUPPORT.md)
