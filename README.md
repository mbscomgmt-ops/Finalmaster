# MBS Phases Site (v1.6)

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
