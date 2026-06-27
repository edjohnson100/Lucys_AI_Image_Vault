======================================================
🚀 SETUP GUIDE: Installing Lucy's AI Image Vault
======================================================
Welcome to Lucy's AI Image Vault!

Because this is a standalone application, you do not need to "install" it like traditional software. You simply place the application file where you want it and turn it on.

------------------------------------------------------
STEP 1: Place the Application
------------------------------------------------------
Move the LucysVault file (.exe for Windows, .app for Mac) to your preferred location.

* Windows Users: You can place this on your Desktop, in a dedicated folder on your C: drive, or even on an external thumb drive.

* Mac Users: For a standard install, drag LucysVault.app to your Applications folder. You can use the main Applications folder or the Applications folder inside your user home folder.

  For Portable Mode, do not place the full portable folder inside Applications. Drag the entire Lucys_Vault folder to a writable local folder, external drive, or thumb drive. Do not run the app directly from the DMG.

------------------------------------------------------
STEP 2: The First Launch
------------------------------------------------------
Double-click the application to open it.

Because this is an independent tool, Windows Defender or macOS Gatekeeper may ask you to confirm that you want to run an unrecognized app.

* Windows Users: Click More Info, then Run Anyway.

* Mac Users: Try Right-Click or Control-Click on LucysVault.app, then choose Open.

  On some versions of macOS, especially newer releases, you may see a warning that the app is "damaged" and should be moved to the Trash. This can happen because the app is unsigned and macOS has quarantined the downloaded file. If this happens, see README_FIRST_MAC.txt for the Terminal command workaround.

Only continue if you downloaded Lucy's AI Image Vault directly from the official GitHub release page and you trust the source.

------------------------------------------------------
STEP 3: Choose Your Vault Location
------------------------------------------------------
When the app opens, it will present you with a Welcome Screen asking where you want to securely store your downloaded artwork and database. You will have three choices:

1. System Default (The "Plug and Play" Method)
   The app automatically creates a hidden, secure folder deep in your system files. This is the safest method and prevents accidental deletion.

2. Documents Mode (The "Easy Access" Method)
   The app will automatically create a new "LucysVault" folder right inside your computer's standard Documents folder so you can easily browse your raw files.

   ⚠️ THE CLOUD SYNC TRAP: Do NOT use this option if your Documents folder is being actively synced or backed up by iCloud Drive, OneDrive, Dropbox, Google Drive, or a similar cloud-sync service. Running a live database inside a syncing folder can cause file conflicts, database issues, or unexpected behavior.

3. Portable Mode (The "Thumb Drive" Method)
   The app will build your database and image folders directly next to wherever you placed the application file in Step 1. This is useful if you placed the app on an external hard drive or thumb drive and want everything kept together.

Once you click your choice, the application will automatically build your folders and launch your gallery!

------------------------------------------------------
STEP 4: Run Your First Cloud Sync
------------------------------------------------------
Head to the Control Center tab at the top of the app to get started.

RECOMMENDED FIRST SYNC: Set the "Quick Sync pages" input to 1 and click Quick Sync. This captures your 32 most recent designs from Artistly and downloads the images — enough real data to explore the gallery, try the filters, and get comfortable with the app before committing to a larger sync. Once you've had a look around, you can always come back and run a bigger sync to bring in the rest of your library.

Watch the Task Console panel at the bottom for progress updates. When the sync finishes, click Refresh Data in the left sidebar to see your newly synced image count. Then, click the Main Gallery button in the top navigation to view your images.

------------------------------------------------------
MAC USERS ONLY: App Management Permission
------------------------------------------------------
The first time you run a sync, macOS will ask you to approve App Management permission for the app. This is required because the app uses a built-in browser to connect to Artistly.

You may see the prompt as a system dialog, or you may need to go to:

System Settings → Privacy & Security → App Management

You must close Lucy's AI Image Vault, approve the security setting, and relaunch the app. Once approved, syncs will run without further prompts going forward.
