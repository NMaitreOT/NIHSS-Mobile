# Updating NIHSS Mobile on GitHub Pages

Repository: `nmaitreot/NIHSS-Mobile`

## Easiest method: GitHub website

1. Download and unzip the V4 GitHub Pages package.
2. Open your `NIHSS-Mobile` repository on GitHub.
3. Select **Add file > Upload files**.
4. Drag **all files from inside the unzipped V4 folder** into the upload area. Do not upload the ZIP itself and do not put the files inside a new subfolder.
5. GitHub will identify files with the same names as replacements/updates. Keep `index.html`, `sw.js`, `manifest.webmanifest`, icons, stimulus images, and `.nojekyll` at the repository root.
6. In the commit message, enter something such as `Update NIHSS Mobile to V4 - longitudinal tracking`.
7. Choose **Commit directly to the main branch** and select **Commit changes**.
8. Open the repository **Actions** tab and wait for the Pages deployment to show a green check.
9. Open `https://nmaitreot.github.io/NIHSS-Mobile/` in Safari and refresh it.
10. If the Home Screen app still shows V3, fully close it and reopen it. If necessary, open the website once in Safari while online, refresh, then reopen the Home Screen app so the updated service worker can cache V4.

## Important data behavior

Longitudinal history is stored locally in the browser/app on that device. It is NOT committed to GitHub and is NOT synchronized between devices. Use the app's Export function before clearing Safari website data, deleting the Home Screen web app, or moving to another device. Import the exported JSON file on the destination device.
