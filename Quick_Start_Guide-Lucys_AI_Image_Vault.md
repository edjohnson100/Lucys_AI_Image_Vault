# 🚀 SETUP GUIDE: Installing Lucy's AI Image Vault

Welcome to Lucy's AI Image Vault! This application operates completely independently on your computer without a traditional software installation process. You simply place the file where you want it and turn it on.

---

### STEP 1: Position the Application

Move the LucysVault application file (`.exe` for Windows, or the `.app` package located inside your downloaded `.dmg` disk image for Mac) to its permanent home:

*   **For Desktop Access:** Create a dedicated folder on your Desktop named `Lucy's AI Image Vault` and place the application file inside it. This keeps your workspace clean and tidy. *(⚠️ Note: If you plan on keeping your vault completely self-contained inside this folder, please review the Cloud Backup Trap warning in STEP 3 before proceeding!)*
*   **For Standard Storage:** Windows users can place the file inside a dedicated folder on their main `C:` drive. Mac users can drag the application icon straight into their computer's standard **Applications** folder.
*   **For On-The-Go Storage:** If you want to use the application from an external hard drive or a portable thumb drive, move the application file directly into a folder on that specific device.

---

### STEP 2: The First Launch

Double-click the application icon to open it.

> **Security Verification:** Because this is an independent, community-built tool, a system security warning **may be displayed** before running it the first time. On Windows, select *More Info* and choose *Run Anyway*. On Mac, hold the **Control** key, click the application icon, and choose **Open**.
>
> *🍏 Mac Users (macOS Tahoe): If you are running new updates or consecutive builds, you may experience a quirk where your application permissions settings get reset. I have included a short video demo with your download showing exactly what this looks like on macOS Tahoe and how to quickly clear it!*

---

### STEP 3: Choose Your Storage Style

When the application window loads, a welcome screen will appear asking you where you want to securely save your downloaded artwork collection and index records. Select the button that matches how you want the application to operate:

1.  **System Default (Safest Method)**
    The application will automatically build a secure, hidden data repository deep within your computer's internal system folders. This is the safest setting because it completely isolates your gallery files and prevents accidental deletion.
2.  **Documents Mode (Easy Access Method)**
    The application will automatically create a brand new visible folder called `LucysVault` inside your personal computer's standard **Documents** folder. This allows you to easily browse through your raw image files directly.
    *   *⚠️ THE CLOUD BACKUP TRAP: Do not select this option if your computer's Documents folder automatically syncs to a service like iCloud Drive, OneDrive, or Dropbox. Running an active database inside a cloud-syncing folder will cause saving conflicts and corrupt your gallery history.*
3.  **Portable Mode (Thumb Drive Method - Personally Recommended)**
    The application will build its entire storage ecosystem right next to the application file itself inside the folder you chose in Step 1. This is ideal if you are running the app from an external hard drive, keeping your data entirely self-contained.

Once you click your choice on screen, the gallery will instantly construct its storage layout, establish the background file paths, and launch your visual dashboard!

---

### STEP 4: Running Your First Cloud Sync

Your gallery vault is ready — now let's fill it with your Artistly designs! Click the **Control Center** tab at the top of the app to get started.

> ⚡ **Get Up and Running Fast:** Want to see the app in action right away? Set the **Quick Sync pages** input to `1` and click **Quick Sync**. This captures your 32 most recent designs from your personal Artistly library and downloads the images — enough real data to explore the gallery, try the filters, and get comfortable with the app before committing to a larger sync. Once you've had a look around, you can always come back and run a bigger sync to bring in the rest of your library.

In the **Cloud Sync** card, you have two options:

*   **Quick Sync** — scans your most recent ~128 designs and downloads their images. This is the recommended starting point: fast, and it lets you see the gallery working right away.
*   **Full Audit** — scans your entire Artistly library from start to finish. Use this for a complete archive. Expect it to take several minutes if you have a large collection.

> **Tip for large libraries:** Before clicking either button, check the **Skip image download pass** checkbox. This pulls in all your design metadata first without downloading image files, which is much faster. You can then batch-download the actual images at your own pace using the **Direct Download** button in the Image Downloads card.

Click your chosen sync button. The app will open a browser window and navigate to your Artistly account automatically.

*   If your Artistly session is still active, the sync begins immediately with no input needed.
*   If you have been logged out, the browser will pause at the login page — sign in normally and the sync will resume on its own.

Watch the **System Terminal** at the bottom of the screen for live progress. When the sync finishes, click **Refresh Data** in the left sidebar to see your newly synced gallery!

> *🍏 Mac Users: Cloud sync uses a bundled browser to connect to Artistly. The first time you run a sync, macOS may prompt you for **App Management** permission — grant it when asked and then close and re-open Lucy's AI Image Vault, as this permission is required for the sync feature to work. I have included a short video demo with your download showing exactly what this looks like and how to clear it quickly.*
