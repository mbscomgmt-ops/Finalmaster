# MBS Phases Site (v3.3)

A single-file, iPad/iPhone-friendly phases page with:
- Phase bubbles with live progress bars
- Locked later phases until the previous hits 100% (toggle-able in Dev mode)
- Timeline + checklist for each phase
- LocalStorage persistence
- Version stamp in footer

## Quick Start
1. Open `index.html` in any browser.

## Deploy to GitHub Pages
1. Create a new repo (e.g., `mbs-phases-site`).
2. Upload `index.html` to the repository's root.
3. In repo **Settings → Pages**, set:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (or `master`) / root
4. Your site will appear at the Pages URL shown there.

## Deploy to Netlify
1. Drag-and-drop the folder onto Netlify, or link your repo.
2. Build command: *None* (it's static).
3. Publish directory: `/`.

## Customize Phases
Edit the `PHASES` array in the `<script>` tag near the bottom of `index.html`:
- Change `name`, `icon`, and the `timeline`/`tasks` arrays.
- Checkboxes update the progress bar automatically.
- To remove gating, click **Toggle lock (dev)** in the page.

## Reset Progress
Use the **Reset progress** button or clear your browser's LocalStorage key: `mbs_phase_progress_v11`.


## Logo
Replace `logo.svg` with your company logo using the same filename to update the header.


## Services & Metrics Page
Open `services.html` for a live metrics dashboard:
- Editable JSON box with LocalStorage persistence
- Metric tiles (Bookings, AOV, Completion Time, Deposit Rate, Conversion, On-time Arrival, Revenue MTD/YTD)
- Two sparkline charts (Bookings, Revenue) over the last 12 weeks
- Linked from the header on all pages


### Extras in v3.3
- Jobs by Service Type (bar)
- Revenue by Region (donut)
- Tech Utilization (bar)
- Prefilled defaults tuned for MBS Handy Services

- Added Back to Phases link in Services page hero section.

- Updated header nav: Services & Monday.com links appear side-by-side as a right-side menu.

- Added smooth hover underline animation to Services & Monday.com nav links (all pages).

- Expanded nav menu: added placeholders for Community & Real Estate (future MBS brand sections).

- Added **Home** label in nav menu, pointing to Phases page (index.html).

- Removed Monday.com link from landing page body (kept in nav only).

- Tidied landing page layout: removed empty header actions and adjusted hero spacing after Monday.com removal.

- Converted right-side menu into a dropdown on all pages; added **Monday.com** and **QuickBooks** (both open in new tabs).

- Replaced dropdown text label with a hamburger icon button in the header.

- Upgraded Phases checklist: nested subtasks, per-task mini progress, and overall leaf-based progress bars.

- New blurred-photo background with translucent UI so the image shines through.
- Replaced dropdown menu with a right-side slide-in drawer; trigger is a minimal icon (no button chrome).
- Removed logo background fill for cleaner header.

- Replaced abstract background with provided custom background photo (`bg.png`).

- Added a dark overlay gradient on top of the background photo for clearer text/box contrast.

- Fixed background layering: photo + overlay are now fully behind all content (z-index corrected).

- Repair: ensured phases sections and side menu exist; corrected z-index and reinserted toggle scripts where missing.
