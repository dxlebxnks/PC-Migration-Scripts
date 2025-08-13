# PC Migration Scripts

This repository contains PowerShell scripts to assist with migrating users from an old PC to a new PC. It helps IT admins backup and restore:

- Full user profile data (Documents, Desktop, AppData)
- Browser bookmarks (Chrome, Edge, Firefox)
- Outlook email signatures
- Printer configurations

## 🛠️ Usage Overview

### 1. Backup on Old PC
Run the following scripts before moving to the new PC:

```powershell
.\Scripts\Backup-UserData.ps1
.\Scripts\Backup-Bookmarks.ps1
.\Scripts\Backup-OutlookSignatures.ps1
.\Scripts\Backup-Printers.ps1

The scripts will create a D:\Migration folder (or folder of your choice) with all necessary data.

### 2. Restore on New PC

After imaging the new PC and logging in as the user:
