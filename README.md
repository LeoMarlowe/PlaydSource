# Playd SideStore Source

This is a SideStore source for the Playd game tracker app.

## Add This Source to SideStore

1. Copy this URL:
   ```
   https://raw.githubusercontent.com/LeoMarlowe/PlaydSource/main/apps.json
   ```

2. Open **SideStore** on your iPhone

3. Go to **Browse** tab → **Sources** (top left)

4. Tap **+** and paste the URL

5. The "Playd Apps" source will appear

6. Find **Playd** and tap **Get**

## For Developers: How to Update

### After each Codemagic build:

1. Download the IPA from Codemagic

2. Upload to GitHub Releases:
   - Go to https://github.com/LeoMarlowe/PlaydSource/releases
   - Create new release with tag `v1.4.x`
   - Upload `Playd.ipa` and `Playd.exe` on that same release, plus `Playd-<version>.sha256` for the exe

3. Update `apps.json`:
   - Update `version` and `buildVersion`
   - Update `date` to today
   - Update `localizedDescription` with changelog
   - Update `downloadURL` to new release URL

4. Commit and push

Users will see the update in AltStore automatically!

## Files in this repo

- `apps.json` - The AltStore source file
- `icon.png` - App icon (512x512 recommended)
- `header.png` - Optional header image for source page
- `README.md` - This file
