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

1. Collect the validated iOS IPA from Bitrise and the signed Android APK and packaged Windows executable from their release builds.
2. Publish `Playd.ipa`, `Playd.apk`, and `Playd.exe` together in the `v<version>` GitHub release. Mark it latest so the Windows updater picks it up.
3. Add the iOS release at the top of `apps[0].versions` in `apps.json`. Use the IPA's `version`, `buildVersion`, and byte `size`, GitHub's UTC `publishedAt` for `date`, the versioned IPA URL for `downloadURL`, and the iOS notes for `localizedDescription`.
4. Push the feed update to `main` after the release assets are public. SideStore reads the feed from that branch.

## Files in this repo

- `apps.json` - The AltStore source file
- `icon.png` - App icon (512x512 recommended)
- `header.png` - Optional header image for source page
- `README.md` - This file
