# Played AltStore Source

This is an AltStore source for the Played game tracker app.

## Add This Source to AltStore

1. Copy this URL:
   ```
   https://raw.githubusercontent.com/LeoMarlowe/PlayedSource/main/apps.json
   ```

2. Open **AltStore** on your iPhone

3. Go to **Browse** tab → **Sources** (top left)

4. Tap **+** and paste the URL

5. The "Played Apps" source will appear

6. Find **Played** and tap **Get**

## For Developers: How to Update

### After each Codemagic build:

1. Download the IPA from Codemagic

2. Upload to GitHub Releases:
   - Go to https://github.com/LeoMarlowe/PlayedSource/releases
   - Create new release with tag `v1.4.x`
   - Upload the IPA file

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
