# CursorAI Agent for Mac

Menu-bar helper that lets you control **Cursor** from the **Cursor Mobile** iOS app.  
Runs `cursor-agent` locally on your Mac and syncs responses back to the phone.

---

## Download

👉 **Latest build:** [Releases › Latest](../../releases/latest)

Download the `.dmg` or `.zip` from the latest release.

---

## Requirements

- macOS 13+ (Ventura or newer)
- Cursor desktop app installed
- `cursor-agent` CLI installed and working in Terminal
- Cursor Mobile iOS app (same Cursor account)

---

## Install

1. Download `CursorAI Agent for Mac.dmg` (or `.zip`) from **Releases**.
2. DMG: open and drag **CursorAI Agent for Mac.app** to **Applications**.  
   ZIP: unzip and move the `.app` to **Applications**.
3. Open the app from Applications → confirm the “Downloaded from internet” dialog.
4. You’ll see the app’s icon appear in the **menu bar**.

---

## First-time setup

1. Make sure `cursor-agent` works in Terminal:

   ```bash
   cursor-agent --version
   ```

2. Click the menu-bar icon:
   - Pick your project folder (repo) for running commands.
   - If the app shows a **“Connect to Cursor”** / login button, click it once and finish login.

3. Open **Cursor Mobile** on iOS and make sure you’re signed in with the same Apple ID (for sync).

---

## Usage

- Use the **Cursor Mobile** app to send prompts/commands.
- The Mac agent:
  - Receives the message,
  - Runs `cursor-agent` in the selected project folder,
  - Syncs the result back to the shared chat.

If you see an error about `cursor-agent` or chat creation, double-check:

- `cursor-agent` is installed and authenticated (`cursor login` in Terminal).
- A project folder is selected in the menu-bar popup.

---

## Support

If something doesn’t work:

1. Grab the latest version from **Releases**.
2. Open an Issue on this repo with:
   - macOS version,
   - app version,
   - screenshot of the error.
