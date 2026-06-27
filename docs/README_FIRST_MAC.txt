======================================================
🍎 MAC FIRST LAUNCH NOTES: Lucy's AI Image Vault
======================================================

Lucy's AI Image Vault for Mac is currently unsigned. That means macOS may block it the first time you try to open it.

Only continue with these steps if you downloaded Lucy's AI Image Vault directly from the official GitHub release page and you trust the source.

------------------------------------------------------
STANDARD MAC FIRST-LAUNCH METHOD
------------------------------------------------------
1. Open the DMG.
2. Drag LucysVault.app out of the DMG.
   Recommended locations:
   - Applications
   - your user Applications folder
   - another writable local folder

3. Do not run the app directly from the DMG.
4. Right-Click or Control-Click LucysVault.app.
5. Choose Open.
6. If macOS asks for confirmation, choose Open again.

On some macOS versions, this may be enough.

------------------------------------------------------
IF MACOS SAYS THE APP IS "DAMAGED"
------------------------------------------------------
On some versions of macOS, especially newer releases, you may see a message like:

"LucysVault.app" is damaged and can't be opened. You should move it to the Trash.

This does not always mean the download is actually damaged. It can happen because macOS quarantined the downloaded app because it is unsigned.

If you trust the source, you can remove the quarantine flag manually.

------------------------------------------------------
TERMINAL METHOD: REMOVE THE QUARANTINE FLAG
------------------------------------------------------
1. In Finder, locate the folder that contains LucysVault.app.

2. Right-Click or Control-Click the folder itself.

3. Choose:

   New Terminal at Folder

   If you do not see that option, look under:

   Services → New Terminal at Folder

4. A Terminal window should open already pointed at that folder.

5. Run this command:

   xattr -dr com.apple.quarantine "LucysVault.app"

6. Press Return.

7. Go back to Finder and open LucysVault.app again.

------------------------------------------------------
PORTABLE-FRIENDLY DMG NOTES
------------------------------------------------------
If you downloaded the portable-friendly DMG, it contains a single Lucys_Vault folder.

Drag the entire Lucys_Vault folder to a writable local folder, external drive, or thumb drive before opening the app.

Do not run Portable Mode directly from the DMG.
Do not place the portable folder inside a cloud-synced folder.
Do not place the portable folder inside Applications.

Good Portable Mode locations include:
- an external drive
- a thumb drive
- a dedicated local folder that is not cloud-synced

------------------------------------------------------
CLOUD SYNC WARNING
------------------------------------------------------
Do not place the live vault database or config files inside folders actively synced by iCloud Drive, OneDrive, Dropbox, Google Drive, or similar services.

If your Desktop and Documents folders are synced by iCloud Drive, choose System Default on first launch.

System Default is the recommended storage option for most Mac users.

------------------------------------------------------
WHAT THIS COMMAND DOES
------------------------------------------------------
The xattr command above removes the macOS quarantine flag from the app.

It does not grant special permissions.
It does not bypass App Management permissions.
It does not change your Artistly account.
It only tells macOS not to treat this downloaded app as quarantined.

After the app opens, macOS may still ask for normal permissions later, such as App Management, during the first sync.
