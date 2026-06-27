======================================================
🚀 PORTABLE MODE GUIDE: Lucy's AI Image Vault
======================================================

Portable Mode keeps Lucy's AI Image Vault and its working data together in one folder. This is useful when you want to run the app from an external drive, thumb drive, or another local folder you manage yourself.

IMPORTANT:
Portable Mode is for a writable local folder or external drive.
Do not run Portable Mode directly from a ZIP file, directly from a Mac DMG, or from a cloud-synced folder.

------------------------------------------------------
WHAT IS INCLUDED IN THE PORTABLE-FRIENDLY PACKAGE?
------------------------------------------------------

The portable-friendly download contains one folder:

   Lucys_Vault

Keep this folder together. It is designed so you can drag the whole folder to the location where you want to run the app.

Inside the folder you may find:

   LucysVault.exe              Windows app
   LucysVault.app              Mac app
   Documentation and Licenses  Docs, license files, and notices

When you choose Portable Mode on first launch, Lucy's AI Image Vault will create its working database, configuration files, and image folders next to the application inside the portable folder.

------------------------------------------------------
WHERE SHOULD I PUT THE PORTABLE FOLDER?
------------------------------------------------------

Good locations:

   Windows:
   - A dedicated folder on your C: drive
   - An external USB drive
   - A thumb drive
   - A local folder that is not cloud-synced

   Mac:
   - A dedicated local folder in your home folder
   - An external USB drive
   - A thumb drive
   - A local folder that is not cloud-synced

Avoid these locations for Portable Mode:

   - iCloud Drive
   - OneDrive
   - Dropbox
   - Google Drive
   - Any actively cloud-synced folder
   - A Mac DMG disk image
   - A ZIP file or compressed folder
   - A read-only drive or folder

Cloud syncing can interfere with the app while it is writing to its live database and configuration files. Use cloud storage for backup copies or exported files, not for the active portable vault.

------------------------------------------------------
WINDOWS PORTABLE MODE TIPS
------------------------------------------------------

1. Move the Lucys_Vault folder to the location where you want to run it.

   Examples:
      C:\Lucys_Vault
      D:\Lucys_Vault
      E:\Lucys_Vault

2. Open the folder.

3. Double-click LucysVault.exe.

4. If Windows Defender SmartScreen appears:
   - Click More info
   - Click Run anyway

5. On the first-run screen, choose:

      Portable Mode

6. The app will create its working data inside the Lucys_Vault folder.

7. If you are running from a USB drive or thumb drive, always close the app before ejecting or unplugging the drive.

------------------------------------------------------
MAC PORTABLE MODE TIPS
------------------------------------------------------

1. Open the portable-friendly DMG.

2. Drag the entire Lucys_Vault folder out of the DMG.

   Good choices:
      - An external drive
      - A thumb drive
      - A local folder in your home folder

3. Do not run the app directly from the DMG.

4. Open the copied Lucys_Vault folder.

5. Open LucysVault.app.

6. If macOS shows a security warning because the app is unsigned:
   - Try Control-clicking or right-clicking LucysVault.app
   - Choose Open
   - Confirm that you want to open the app

7. If macOS says the app is "damaged" and should be moved to the Trash, this may be macOS quarantine behavior on newer versions of macOS.

   Only continue if you downloaded Lucy's AI Image Vault directly from the official GitHub release page and you trust the source.

   To remove the quarantine flag:

   a. In Finder, right-click or Control-click the Lucys_Vault folder.
   b. Choose New Terminal at Folder.
      If you do not see it, look under Services > New Terminal at Folder.
   c. In Terminal, run:

      xattr -dr com.apple.quarantine "LucysVault.app"

   d. Press Return.
   e. Try opening LucysVault.app again.

8. On the first-run screen, choose:

      Portable Mode

9. The app will create its working data inside the Lucys_Vault folder.

10. If you are running from a USB drive or thumb drive, always close the app before ejecting or unplugging the drive.

------------------------------------------------------
CROSS-PLATFORM FLASH DRIVE TIPS
------------------------------------------------------

If you want to use the same external drive with both Windows and Mac, format the drive as exFAT.

Recommended flash drive setup:

   Format: exFAT
   Name:   LUCY_VAULT or LUCY_DEMO

Important:
Do not unplug the drive while Lucy's AI Image Vault is running.
Always close the app first, then eject the drive properly.

------------------------------------------------------
BACKUP TIPS
------------------------------------------------------

Portable Mode makes it easy to back up your vault.

To back up your portable vault:

1. Close Lucy's AI Image Vault.
2. Copy the entire Lucys_Vault folder to another drive or backup location.
3. Keep the folder structure intact.

Do not copy only the database file while the app is running.

------------------------------------------------------
WHEN SHOULD I NOT USE PORTABLE MODE?
------------------------------------------------------

Do not use Portable Mode if:

   - You are unsure where to store the app
   - You want the safest setup
   - You use iCloud Drive Desktop and Documents syncing
   - You plan to keep the app inside a cloud-sync folder
   - You do not want to manage the app folder yourself

If you are unsure, choose System Default on the first-run screen instead.

System Default is the safest and easiest option for most users.

------------------------------------------------------
QUICK SUMMARY
------------------------------------------------------

Use Portable Mode when:

   - You want the app and data together
   - You are using an external drive or thumb drive
   - You understand where the files are stored
   - The folder is writable and not cloud-synced

Avoid Portable Mode when:

   - The folder is inside iCloud Drive, OneDrive, Dropbox, or Google Drive
   - The app is still inside a DMG or ZIP
   - The drive may be unplugged while the app is running
   - You want the most hands-off setup

When in doubt, use System Default.
