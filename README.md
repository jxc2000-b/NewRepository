# Notes App

A simple, lightweight note-taking web application with password protection and persistent storage.

## Features

- 🔒 **Password Protection**: Secure access with a hardcoded password
- 📝 **3 Separate Tabs**: Keep different notes organized
- 💾 **Auto-Save**: Notes are automatically saved to browser's localStorage
- ⬇️ **Download Backup**: Export your notes as JSON for safekeeping
- ⬆️ **Upload Restore**: Import previously downloaded backups
- 🔤 **Dynamic Font Sizing**: Font size increases gradually based on time since last edit (resets when you type)

## Usage

1. Open `index.html` in your web browser
2. Enter the password: `123456`
3. Start taking notes!

## Technical Details

- **Storage**: Uses browser's localStorage (no server required)
- **Password**: `123456` (can be changed in the JavaScript code)
- **Font Growth**: Increases by 1px every 2 hours (from 14px to max 24px)
- **Compatibility**: Works in all modern browsers

## How It Works

- Notes are stored locally in your browser
- Each note has its own timestamp
- When you type, the font size resets to minimum and timestamp updates
- Font size gradually increases if note is left untouched
- Download creates a JSON backup file
- Upload restores from a JSON backup file