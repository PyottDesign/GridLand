# GridLand v0.3.8
GridLand is a local Manifest V3 Chrome new-tab extension with adjustable icon grids, pages, groups, custom backgrounds, icon cropping, and profile-local backups.

## Backups and image assets
**Export settings includes uploaded icons, cropped icons, and wallpaper images.**

GridLand stores those local image assets in IndexedDB. Export builds a single JSON backup containing both:

- GridLand layout/settings/pages/groups
- The complete local asset database

If you remove GridLand, reinstall it, and import the backup, those uploaded/cropped images are restored.

## New installation
1. Download to a new permanent folder, for example `Documents\Chrome Extensions\GridLand`.
2. In Chrome, open `chrome://extensions`.
3. Enable **Developer mode** tick box.
4. Click **Load unpacked** button.
5. Select the folder containing `manifest.json`.
6. Open a new tab.

Developer mode must remain enabled while using the unpacked build.

## Permissions
GridLand requests `storage`, `favicon`, and `downloads`. Website host access remains optional and is requested only when you explicitly ask GridLand to inspect a site or load a remote image icons for cropping.