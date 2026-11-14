# Nodex releases

Downloads of **Nodex**, a native Windows spreadsheet where sheets work as functions and node-based
Blueprints replace macros. This repository holds releases only. Each commit here is one release.

## Which file

- **`Nodex-<version>-setup.exe`**: the installed edition. It installs for you alone, with no
  administrator rights needed. It can check for updates: only when you choose Help > Check for
  updates, or, if you turn that on, each time it starts. That's its only internet connection.
- **`Nodex-<version>-portable.zip`**: the portable edition. Unzip anywhere and run `nodex.exe`.
  It has no network code at all and never connects to the internet.

The two editions start with 0.3.0. Version 0.2.0 is one edition, with no update check.

Both open and save `.ndx` workbooks, and read and write Excel `.xlsx` and CSV files.

## Checking a download

Each release has `SHA256SUMS.txt`. In PowerShell:

```powershell
Get-FileHash .\Nodex-0.2.0-setup.exe -Algorithm SHA256
```

The hash should match the line for that file. The installed edition checks this itself before it
runs an update.

The program isn't signed yet, so Windows SmartScreen may warn: choose "More info", then "Run anyway".

Newest: Nodex 0.3.1.
