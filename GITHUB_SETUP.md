# NIHSS Mobile V3 - GitHub Pages Setup

## 1. Create the repository
1. Sign in to GitHub.
2. Select **New repository**.
3. Repository name: `nihss-mobile` (recommended).
4. Choose **Public**.
5. Create the repository.

## 2. Upload the app
Upload ALL files from this package to the root of the repository. `index.html` must remain at the root.

Files:
- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png
- stimulus-1.png
- stimulus-2.png
- stimulus-3.png
- stimulus-4.png

Commit the uploaded files to the `main` branch.

## 3. Enable GitHub Pages
1. In the repository, open **Settings**.
2. Select **Pages** under Code and automation.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Branch: `main`.
5. Folder: `/ (root)`.
6. Select **Save**.

GitHub will publish the site. The address will normally be:
`https://YOUR-USERNAME.github.io/nihss-mobile/`

## 4. Install on iPhone/iPad
1. Open the published HTTPS address in **Safari**.
2. Allow the page to load fully at least once.
3. Tap **Share**.
4. Select **Add to Home Screen**.
5. If offered, enable **Open as Web App**.
6. Tap **Add**.
7. Launch NIHSS from its Home Screen icon.

After the first successful online load, the service worker caches the app assets for offline use. Test offline operation before relying on it where connectivity is limited.

## Updating the app later
Replace the changed files in the same GitHub repository and commit the changes. GitHub Pages will republish automatically. Devices may briefly retain cached files; reopening while online allows the service worker to update its cache.

## Clinical deployment note
This package contains no patient identifier fields and does not maintain a patient/assessment database. Before routine clinical deployment, validate scoring behavior, permitted NT handling, stimulus display, timers, documentation output, accessibility, and offline behavior on the devices/browsers that will actually be used.
