## Lucy's AI Image Vault — v1.0

Artistly.ai automatically deletes your designs after one year. **Lucy's AI Image Vault** is a free desktop app that syncs your full Artistly library to your local machine at full resolution — keeping your work safe permanently, in a fast searchable gallery you own and control.

---

### What's included

**Automated Cloud Sync**
One-click sync connects to your existing Artistly browser session via network interception — no manual exports or API keys. Quick Sync fetches your most recent ~128 designs; Full Audit reconciles your entire library including cloud deletions. Includes configurable page counts, scoped downloads, page-range targeted downloads, and a metadata-only mode for large first-time imports.

**Gallery Browser**
Browse your full archive with filtering by folder, tool, style, favorites, download state, and free-text search. Designs are grouped by generation session under shared headers. Click any image to open the Inspection Workbench for a full-screen view with its prompt, metadata, and action buttons.

**Archive Tab**
Designs deleted from Artistly remain in your local archive — fully browsable, searchable, and exportable. Folder context is preserved at archive time so renames on Artistly never alter your local history.

**Pending Actions**
A dedicated view that collects all designs flagged for bulk move, bulk delete, or ZIP export in one place — review everything before executing.

**Bulk Move & Delete**
Flag designs in the gallery, then execute from the Control Center. Targeted mode uses Artistly's search filter for designs with prompts — fast and precise. Sequential mode handles no-prompt designs via page-batch processing.

**Prompt Library**
A searchable, filterable table of every generation prompt in your archive. Filter by folder, tool, or style; hover any row to see an inline thumbnail preview.

**Gallery Backup**
One-click backup of your full archive — images and database — to any folder or external drive.

**Add External Image**
Import images from other tools or sources into your vault alongside your Artistly designs.

**Edit Metadata**
Archived images support inline editing of tool, style, category, and prompt directly from the Inspection Workbench.

**9 Themes**
Time Capsule Dark, Studio Light, Deep Space, Starbase Medical, Inkwell Comic, Newsprint Comic, Carbon Fiber Maker, Birch Plywood Maker, Purple Paradise.

**Flexible Storage**
Choose System Default, Documents folder, or Portable mode (alongside the `.exe`/`.app`) on first launch. The choice is permanent so your library stays where you put it.

---

### Requirements

- **Windows 10/11** or **macOS 12+**
- Artistly.ai account
- Active Chrome or Edge browser session signed into Artistly (Windows) — cloud sync attaches to your existing session, no passwords stored

### macOS note
Cloud sync features require the **App Management** permission in System Settings → Privacy & Security. The app displays a banner with step-by-step instructions on first launch.

---

### Installation

> **Read this first:** The release bundle includes `README_FIRST.txt` and `Lucys_AI_Image_Vault_Quick_Start_Guide.pdf`. Open `README_FIRST.txt` before launching — it covers the storage location decision you make on first run, which can't be changed later.

#### Windows

1. **Download** `Lucys_Vault_WIN_v1.0.zip` from the assets below and extract it. Move the `Lucys_Vault` folder wherever you'd like to keep the app.
2. **Run:** Open the `Lucys_Vault` folder and double-click `LucysVault.exe`.
3. **First Run:** Choose a storage location for your library. This setting is permanent.

> **Windows SmartScreen:** The app is not code-signed, so Windows Defender may show a warning on first launch. Click **More info → Run anyway** to proceed.

#### macOS

1. **Download** `Lucys_Vault_MAC_v1.0.dmg` from the assets below.
2. **Open the DMG** and drag the `Lucys_Vault` folder to your Desktop, Applications folder, or wherever you'd like to keep it.
3. **Eject** the disk image when done.
4. **First Launch:** Open the `Lucys_Vault` folder, right-click `LucysVault.app`, choose **Open**, then click **Open** in the Gatekeeper dialog. This one-time step is required because the app is not notarized.
5. **First Run:** Choose a storage location for your library on the setup screen.

> **macOS download size:** The Mac build bundles its own Chromium browser for cloud sync automation, which makes it significantly larger than the Windows version. No separate browser installation is needed.

> **App Management Permission:** On first use of any cloud sync feature, macOS will prompt for **App Management** permission (System Settings → Privacy & Security → App Management). This is required to manage the bundled browser processes.
