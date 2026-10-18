# Tasha for Windows

The newest Windows build of Tasha, so you can grab it without a GitHub account or access to anything else. Builds land here automatically from the main Tasha project.

## Install it

1. Open PowerShell. Press the Windows key, type `PowerShell`, press Enter.
2. Paste this in and press Enter.

```powershell
$ProgressPreference = "SilentlyContinue"
Invoke-WebRequest -Uri "https://github.com/practicaljoyco/tasha-downloads/releases/latest/download/Tasha-Windows-setup.exe" -OutFile "$env:USERPROFILE\Downloads\Tasha-Windows-setup.exe"
```

The first line just quiets PowerShell's progress bar, which crawls on big downloads.

3. Run **Tasha-Windows-setup.exe** from your Downloads folder, and follow the installer.

Prefer an `.msi`? Swap `Tasha-Windows-setup.exe` for `Tasha-Windows.msi` in the command above, then run that file instead.

## Why a command, and not a download link

Files that come through a browser get tagged as "downloaded from the internet". Windows then puts a big blue warning in front of apps it hasn't seen enough of yet, and this build is unsigned, so it would get that warning every time. Fetching the file with PowerShell skips the tag, so the installer just runs. Same file either way.

If the warning shows up anyway (say, you grabbed it through the release page): **More info**, then **Run anyway**. That's expected for an unsigned early build.

## What am I installing?

Tasha is a local-first file catalogue. Point it at your folders and it keeps a searchable record of what's in them: names, sizes, kinds, tags, notes. Your files never move, and nothing leaves your machine. No account, no cloud.

## Good to know

- The link above always serves the newest build. Bookmark this page instead of the file.
- Tasha is early software, shared for testing right now. If something misbehaves, send word back the way this link reached you.
