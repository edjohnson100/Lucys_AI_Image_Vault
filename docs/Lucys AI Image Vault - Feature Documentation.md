
# Lucy's AI Image Vault — Feature Documentation

*Version 4.4 · June 2026*

---

**[DRAFT NOTICE]**

 *`This is a draft copy that is a work in progress. It might have broken image placeholders and broken link placeholders.`*

## Overview

Artistly automatically removes designs from your personal library after one year. If you have been using the platform for a while and haven't actively managed your collection, that work — the images, the prompts, the creative history — can quietly disappear.

**Lucy's AI Image Vault** is a free desktop app for Windows and Mac that creates a permanent local copy of your Artistly library on your own computer. It downloads your full-resolution images, preserves your prompts, and organizes everything in a searchable, browsable gallery that belongs to you — no cloud subscription, no expiration date.

Beyond simple backup, the Gallery also gives you tools to manage your cloud library from the app itself: you can flag designs for bulk move or delete, run those operations in one step, and keep your Artistly account organized without clicking through hundreds of individual images and pages.

Everything is stored locally in a vault on your own machine. The app communicates with Artistly only when you initiate a sync or cloud action — it never runs anything in the background without your instruction.

---

## First Launch — Storage Location

The first time you open the app, you choose where your vault lives:

- **System Default** — the standard application data folder for your operating system. Recommended to keep your database and images safe from accidental deletion.
- **Documents Mode** — stores the vault inside your Documents folder, which makes it easy to find. **DO NOT** select this option if your Documents folder syncs to the cloud (iCloud, OneDrive, etc.) It can cause file conflicts.
- **Portable Mode** — stores the vault in the same folder as the app file itself. Use this if you want the entire Gallery on an external drive that you can move between computers.

This choice is permanent and set once. The vault includes both the image database and your downloaded image files.

![The first-launch storage location dialog showing all three storage mode options: System Default, Documents Mode, and Portable Mode](screenshots/first-launch-storage-picker.png)
*Choose where your vault lives — this dialog appears once on first launch.*

---

## Gallery Controls — Left Sidebar

The sidebar is always visible and controls what you see across all views. Changes take effect immediately.

### Refresh Data
The **Refresh Data** button at the top of the sidebar reloads the current view from the vault database. Use this after a sync or import to bring new content into view.

### Stats
Below the refresh button, a small stats panel shows:
- **Total Gallery** — the total number of designs in your collection
- **Showing** — how many are displayed after your active filters are applied

### Search
A text field that filters designs by prompt text. As you type, the gallery updates to show only designs whose prompt contains your search term. A **Clear** button appears when a search is active. Works in the Main Gallery, Prompt Library, and Archive views.

### Filters
Five filters can be used in any combination:

- **Favorites Only** — shows only designs you have starred
- **Hide Archived** — hides designs that have been removed from your Artistly cloud account but are preserved locally (Main Gallery only)
- **Folder** — narrows the view to a specific Artistly folder from your account
- **Tool** — filters by the Artistly tool used to generate the image (e.g., A.I Illustrator, AI Storybook Studio, Consistent Characters, etc.)
- **Style** — filters by the style or category assigned to the design (e.g., Seamless Pattern V2, Human Stylizer, Photo Restoration, etc.)

A **Clear All** button appears at the top of the filter section whenever any filter is active.

### Theme
Nine visual themes are available from a dropdown at the bottom of the sidebar. Your selection is remembered between sessions.

| Theme | Character |
|---|---|
| Time Capsule Dark | Dark gray with indigo accents (default) |
| Studio Light | Clean light gray with blue accents |
| Deep Space | Pure black with gold accents |
| Starbase Medical | Mint green tones with teal accents |
| Inkwell Comic | Deep navy with red accents |
| Newsprint Comic | Warm cream tones with red accents |
| Carbon Fiber Maker | Dark gray with green accents |
| Birch Plywood Maker | Light warm tones with orange accents |
| Purple Paradise | Light lavender tones with purple accents |

![Cycling through several themes in sequence — Deep Space, Birch, Newsprint, and Purple Paradise — each switching the full color palette instantly](screenshots/theme-switcher.gif)
*Nine built-in themes — switch any time from the sidebar. Your choice persists between sessions.*

### Preferred Viewer/Editor
An optional setting where you can enter the full path to an image viewer or editor on your computer (e.g., Affinity Photo, FastStone Image Viewer, Photoshop). A **Browse** button opens a native file picker so you can navigate directly to the application — no need to type the path manually. When set, the **Open** action in the Inspection Workbench will offer your preferred app as a one-click option alongside the system default. The path is remembered between sessions and can be cleared at any time.

![The left sidebar showing active filters — a folder selected, a tool selected, and the Clear All button visible at the top of the filter section](screenshots/sidebar-filters-active.png)
*The sidebar controls what you see across all views. Active filters stack and can be cleared individually or all at once.*

---

## Main Gallery

The default view when you open the app. Displays your entire design collection as a scrollable grid of image cards.

### Selection Groups
Images generated from the same prompt in the same session are grouped together as a cluster and displayed as a single card. If a cluster contains multiple variants, arrow buttons on the card let you step through them, with a counter showing your position (e.g., 2 / 4). Each variant in a cluster has its own independent favorite and flag status.

![Stepping through the variants in a multi-image selection group — arrow buttons advance the counter from 1 / 4 through each variant and loop back to the start](screenshots/variant-navigation.gif)
*Variants generated from the same prompt are grouped into a single card — step through them with the arrow buttons.*

### Pagination
When you have more designs than fit on one screen, a pagination bar appears above and below the grid. You can jump to any page directly or step forward and backward. Navigation wraps — pressing Previous on the first page takes you to the last, and vice versa.

### Image Cards
Each card shows:
- The folder the design belongs to
- The image itself (click to open the Inspection Workbench)
- A **Favorite** button (star icon, top right)
- A 2×2 action button grid with four buttons: **Bulk Move**, **Bulk Delete**, **Delete File**, **ZIP**

Buttons that don't apply to the current image state are shown greyed out and disabled — for example, Bulk Move and Bulk Delete are disabled on archived images, and Delete File is disabled on active (non-archived) images.

### Flagging Designs
Click any active action button on a card to toggle that flag on or off:
- **Bulk Move** — marks the design for a bulk move operation on Artistly
- **Bulk Delete** — marks the design for bulk deletion from Artistly
- **ZIP** — marks the design to be included in a local ZIP export

Any combination of flags can be active at once. Flagged items accumulate in the Pending Actions view until you run the corresponding operation.

![Opening the flag menu on several cards in sequence, toggling Move on the first, ZIP on the second, and Move on the third — each card retaining its flag badge after the menu closes](screenshots/bulk-flagging.gif)
*Flag any combination of Bulk Move, Bulk Delete, and ZIP on each design independently.*

### Inspection Workbench
Clicking any card image opens the Inspection Workbench — a full-detail view for that design.

**Header bar (archived images only):**
- Folder selector — reassign the image to a different folder in your vault
- **Move** button — commits the folder change
- **Edit Metadata** toggle — switches the left panel into an inline editing mode where you can update the Tool, Style, Aspect Ratio, and Prompt. Style has autocomplete suggestions drawn from styles already in your vault. Changes save immediately on clicking **Save**.

**Left panel:**
- Metadata badges: Tool, Style, Aspect ratio, Dimensions, Folder
- Full prompt text (selectable and copyable)
- **Locate in Prompt Library** button — jumps to the Prompt Library filtered to this prompt
- Favorite button and action flags (Move, Delete, ZIP) — same as on the card, but with checkboxes for clarity

Two action buttons run across the bottom of the left panel:

**🚀 Open/Edit Image** — opens the full-resolution image file in an external application. If a Preferred Viewer/Editor is configured in the sidebar, a radio selector appears above the button so you can choose between your system's default app and your preferred app. Your choice persists between sessions.

**📋 Copy Image As** — expands an inline panel where you can copy the full-resolution image file to any folder on your computer with an optional rename. A Browse button opens a native folder picker. If a file with the same name already exists at the destination, the app shows an inline confirmation — you can replace the existing file or cancel and choose a different name or location. After a successful copy, a confirmation message shows the full destination path; clicking it opens that location in your file manager (with the file highlighted on Windows).

**Right panel:**
- Large image display
- Background lightness slider — a horizontal slider below the image that adjusts the panel background from pure black to pure white. Useful for evaluating images with transparency or light-colored edges. The setting persists between sessions and also affects thumbnail backgrounds in the gallery grid and Prompt Library.
- Cluster navigation arrows and variant counter (if applicable)

![The Inspection Workbench showing the left panel with metadata badges, a multi-line prompt, and Open and Copy As buttons, alongside the large image in the right panel](screenshots/inspection-workbench-detail.png)
*The Inspection Workbench — full metadata, full prompt, and direct access to open or copy the image file.*

![Clicking Edit Metadata in the Inspection Workbench header, editing the Style and Prompt fields inline, then saving — the panel returns to read-only with the updated values](screenshots/zoom-edit-metadata.gif)
*Edit Metadata mode — update Tool, Style, Aspect Ratio, and Prompt inline for any archived image.*

---

## Prompt Library

A searchable table of all your designs organized by prompt. Where the Main Gallery is image-first, the Prompt Library is text-first — useful when you want to find a specific prompt or copy it for reuse.

### Table Layout
Each row shows:
- A small thumbnail image (hover over it to see a 4× zoom preview — the zoomed image pops above the table boundary so it is never cut off by the list edge)
- Tag badges for Tool, Style, and Aspect Ratio
- The full prompt text — truncated at three lines by default, with a **more...** link to expand it. Prompt text is selectable and copyable directly from the table.
- A **Copy Prompt** button — copies the prompt to your clipboard in one click
- A **Favorite** button — the same favorite flag used everywhere in the Gallery
- A **Find in Gallery** button — switches to the Main Gallery and searches using this prompt, so you can quickly see all images that match

The same Search and Filter controls in the sidebar work in the Prompt Library, so you can narrow by folder, tool, style, or keyword just as you would in the gallery.

![Hovering over thumbnails in the Prompt Library table — the zoomed preview pops above the table boundary without clipping, even for rows in the middle of the list](screenshots/prompt-library-hover.gif)
*Hover over any thumbnail in the Prompt Library for a 4× preview — it always pops above the table edge so nothing is cut off.*

---

## Pending Actions

A filtered view of the Main Gallery showing only designs that have been flagged for Move, Delete, or ZIP. No new controls — it is the same gallery grid, just pre-filtered.

Use this view to review what you have queued before running a bulk cloud operation from the Control Center. You can adjust or remove flags here the same way you set them.

---

## Archive

Shows designs that have been removed from your Artistly cloud account but are preserved in your local gallery vault. These are images that exist only on your computer — the cloud copy is gone.

Archived designs are visible from the Main Gallery by default (use the **Hide Archived** filter to remove them from the view). They are full citizens of the vault: searchable, browsable, favoritable, and exportable.

### Archive Actions
From the Inspection Workbench, archived images have a dedicated actions panel:
- **Flag for ZIP Download** — include this image in a local ZIP export

Change Folder and Edit Metadata controls are in the modal header (see Inspection Workbench above).

From the card grid directly, archived images show:
- **Delete File** — permanently removes the image file from your computer. This is irreversible and asks for confirmation.
- **ZIP checkbox** — same ZIP flag as above

### Add External Image
The Archive tab includes an **Add External Image** button for importing images you generated outside of Artistly (from other AI tools, or local edits) into your vault. A form lets you enter the file path, metadata (tool, style, aspect ratio, folder), creation date, and prompt. The Style field offers autocomplete suggestions drawn from styles already in your vault, while still accepting any free-form value. The image is copied into your vault and treated like any other archived design.

![Filling in the Add External Image form — selecting a file, watching the dimensions auto-populate, then typing in the Style field and selecting an autocomplete suggestion before submitting](screenshots/add-external-image.gif)
*Add External Image — import images from any source into your vault with full metadata and autocomplete style suggestions.*

---

## Control Center

The operational hub for syncing with Artistly, running bulk actions, managing backups, and monitoring what the app is doing. Cloud operations in the Control Center run live and display output in the terminal at the bottom of the screen.

The sidebar filters are disabled while the Control Center is active.

![The full Control Center view showing all cards — Cloud Sync, Image Downloads, Bulk Move, Bulk Delete, Gallery Backup, Local Exports, and Storage Stats — with the System Terminal visible at the bottom](screenshots/control-center-overview.png)
*The Control Center — all cloud and local operations in one place, with a live terminal at the bottom.*

### Cloud Sync
Keeps your vault database up to date with your current Artistly library.
- **Quick Sync** — scans your most recent Artistly pages and pulls in new or changed designs. Use this for day-to-day refreshes.
- **Full Audit** — a thorough end-to-end reconciliation of your entire Artistly account against the vault. Slower but more complete; recommended for first use and periodic check-ins.

**Quick Sync pages** — a number input (1–4) that sets how many pages of recent designs Quick Sync will scan. Each page covers roughly 32 designs, so the default of 4 pages captures approximately your 128 most recently created designs. If you sync frequently and only want to pull in the very latest work, reducing this to 1 or 2 pages makes Quick Sync faster. The setting is remembered between sessions.

**Skip image download pass** — a checkbox below the two sync buttons. When checked, both Quick Sync and Full Audit update the metadata database only, without downloading any image files. This is the recommended approach when setting up the Gallery for the first time with a large library: run a metadata-only sync to register all your designs, then use the **Direct Download** button in the Image Downloads card to fetch the actual image files in manageable batches at your own pace. The setting is remembered between sessions.

**Download batch limit** — a number input that caps how many images the download pass will process in a single run. Leave it blank to download everything. If you have a very large library and want to spread the initial image download across multiple sessions, enter a number here (for example, 500). The setting is remembered between sessions and applies to both the sync chain download pass and the standalone Direct Download in the Image Downloads card.

At the bottom of the Cloud Sync card, a **Last sync** line shows the date and time of the most recent completed sync, the sync type (Quick or Full), and the total number of designs recorded at that time. This updates automatically after each sync completes.

### Image Downloads
Two standalone download options, available separately from the sync chain:
- **Direct Download** — the primary download path. Fetches images directly from Artistly's CDN without opening a browser. Fast and reliable for most users. Respects the Download batch limit setting.
- **Bulk Download** — a browser-based fallback for cases where CDN URLs have expired and Direct Download can no longer retrieve the files. Uses Playwright to automate Artistly's own ZIP download flow.

Use Direct Download for normal day-to-day use. Switch to Bulk Download only if you have a backlog of images that Direct Download reports as unavailable.

**Page range** — two optional inputs in the Image Downloads card (**Pages** start and end) let you target a specific range of pages within your library when running a standalone Direct Download. Pages are ordered newest-first, so page 1 is your most recently created designs. If you enter only a start page, the end defaults to the same page (one page). This is useful for filling in a specific section of your archive or prioritizing recently generated work without re-processing the entire backlog. Page range applies to the standalone Direct Download only — Quick Sync and Full Audit are unaffected. The setting is remembered between sessions.

### Bulk Move
Executes move operations on designs you have flagged for Move.
- **Smart Prep** — a helper tool that analyzes your gallery for images that are "uncategorized" (assigned to the default folder when created), grouped by tool and style used. It prompts for the group of images you want to process for a bulk move, making it easy to clean up your folder organization in a structured, deliberate way.
- **Targeted Move** — runs the move operation on flagged designs that have a "Style" applied in the image's metadata. This is a very fast operation due to the way Artistly stores metadata.
- **Sequential Move** — runs the move operation on flagged designs without a specific "Style" in the metadata. This is a bit slower operation because the app has to do a sequential search one "Load More" page at a time until the image(s) are found and marked for the bulk move.

Buttons show a count badge when flagged items are waiting.

### Bulk Delete
Executes delete operations on designs you have flagged for Delete.
- **Targeted Delete** — finds and marks designs for a bulk delete operation in the same way the Targeted Move works.
- **Sequential Delete** — finds and marks designs for a bulk delete operation in the same way the Sequential Move works.

Buttons show a count badge when flagged items are waiting.

---
***Important Note***

All **Bulk Move** and **Bulk Delete** operations require human intervention to complete the operations. The app helps find and mark items for a move or delete operation, but you have to confirm that action.

---


### Gallery Backup
- **Backup** — copies your entire vault to a configured backup destination (an external drive, network share, or any local folder). The backup is one-way and non-destructive: new and changed files are copied to the destination, and nothing is ever deleted from it.
- **Settings** — configure the backup destination path using a native folder picker. The chosen path is saved for future runs.

### Local Exports
- **Download ZIP** — packages all designs flagged for ZIP into a single ZIP file. The button shows a count badge when flagged items are ready. When the export completes, a confirmation dialog shows the full save path and offers an **Open Exports Folder** button to go directly to the file in your file manager.
- **Exports Folder** — the current export destination path is always displayed in the card. By default, ZIP files are saved to an `Exports` folder in the app's data directory. A **Browse** button lets you choose any folder on your computer as the export destination — the dialog opens to the currently configured folder, or to the default location if none is set. The chosen folder is remembered between sessions and can be cleared to revert to the default.

### Storage Stats
A live summary of how much space your vault is using:
- Database file size
- Image folder size
- Total number of downloaded images
- Total number of archived images

A **Recalculate** button refreshes the stats on demand.

### System Terminal
A live console at the bottom of the Control Center that displays output from any running operation — sync logs, move confirmations, error messages, and progress indicators. Prompts for input from the user as required for some operations. Output is color-coded and monospaced. The terminal can be cleared at any time, and its contents are selectable for copying.

![The System Terminal streaming color-coded log output during a live Quick Sync — design names, folder assignments, and a running count of designs processed](screenshots/sync-terminal.gif)
*The System Terminal streams live output for every operation — logs, confirmations, errors, and interactive prompts.*

---

## First-Run Notices

Two informational notices appear during early use of the app:

**Welcome screen** — on first launch, walks you through the storage location choice before the Gallery opens.

**Community Tool Notice** — the first time you run any cloud operation (sync, move, delete), a one-time notice explains that this is a community-built tool with no official affiliation with Artistly, and that cloud automation carries inherent risks. Accepting this notice stores your acknowledgment so it does not appear again.

**Chrome/Edge "unsupported flag" banner** — when a cloud sync or bulk action opens a browser window, Chrome or Edge may display a yellow banner reading "You are using an unsupported command-line flag: --no-sandbox. Stability and security will suffer." This is expected behavior. Playwright requires this flag to attach to your existing browser profile and login session. It does not represent a security issue — the browser is only navigating to `app.artistly.ai`, not browsing the open web. You can dismiss the banner; it may reappear on subsequent runs.
