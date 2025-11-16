# Notes App

Lightweight note-taking web app with iPhone-style PIN, 3 tabs, auto-save, and aggressive font growth.

## Quick Start

**Local:**
```bash
# Open directly
open index.html

# Or serve with Python
python3 -m http.server 8080
# Visit http://localhost:8080
```

**Deploy:**
- GitHub Pages: Push to `gh-pages` branch
- Netlify/Vercel: Drag & drop `index.html`
- Any static host: Upload `index.html`

**PIN:** `123456`

## Features

- 🔒 iPhone-style 6-digit PIN
- 📝 3 separate note tabs
- 💾 Auto-save to localStorage
- ⬇️ Download/Upload JSON backups
- 📈 Font grows 14px→100px over time (doesn't reset on typing)

## Testing Notes

**Authentication:**
- ✅ PIN blocks fill as you type
- ✅ Auto-unlock at 6 digits
- ✅ Wrong PIN shows error + shake
- ✅ Keyboard entry works

**Notes:**
- ✅ Content persists after reload
- ✅ Tab switching preserves content
- ✅ Auto-save on every keystroke
- ✅ All 3 tabs work independently

**Font Growth:**
- ✅ Starts at 14px
- ✅ Grows 1px per 2 hours (max 100px)
- ✅ Does NOT reset when typing
- ✅ Only resets on full deletion

**Backup/Restore:**
- ✅ Download creates valid JSON
- ✅ Upload restores all 3 notes
- ✅ Timestamps preserved

**Browser Testing:**
- ✅ Chrome/Edge/Safari/Firefox
- ✅ Mobile responsive
- ✅ localStorage works across sessions