# IPRESS — GitHub Pages edition

This is the upload-ready static IPRESS website. No npm installation or build is needed. It includes the interactive 3D camera, the seven correctly ordered characters, original photographs, motion controls, creative-field explorer, and official community links.

## Publish for free on GitHub Pages

1. Sign in to GitHub and create a **public** repository named `ipress` (or use an empty public repository you own). GitHub Free supports Pages on public repositories.
2. Extract this ZIP. Open the extracted `ipress-github-pages` folder.
3. In the repository, choose **Add file → Upload files** (or **uploading an existing file** on an empty repository). Upload the **contents** of this folder, including the `assets` and `vendor` folders. Do not upload the ZIP itself or put everything inside an extra enclosing folder. `index.html` must appear in the repository root.
4. Commit the upload to `main`.
5. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**. Click **Save**.
6. After deployment finishes, use **Visit site** on the Pages settings screen. A repository named `ipress` normally appears at `https://YOUR-USERNAME.github.io/ipress/`. Publication may take up to ten minutes.

All local paths are relative, so both a project URL (`/ipress/`) and a user-site URL (`/`) work. The included `.nojekyll` avoids unnecessary Jekyll processing. If your upload interface omits it, create an empty file with that name in the repository root.

## Recruitment: understand this before inviting applicants

**GitHub Pages hosts static websites; it cannot run the existing server or database.** This export therefore links visitors to the real application form at:

https://ipress-universe.briny-tern-7089.chatgpt.site/#apply

The administrator link also points to the existing protected administration page. No applicant data, administrator identities, database, secret, or authentication credential is bundled in this export. The GitHub page does not collect personal details or display a fake successful submission. The six exploratory interest choices stay in the page and are not sent; applicants confirm them in the hosted form.

**The existing application site was owner-private when this package was prepared.** Students cannot submit there until its audience is opened. The visible notice “Ouverture aux étudiants en préparation” reflects that state.

To keep the existing working application system:

1. Ask the site owner to make the existing IPRESS application Site public. This is a separate access change; publishing GitHub Pages does not change it.
2. Verify as an ordinary student that the form is accessible and saves a real application, and that the administrator page stays restricted.
3. Once this succeeds, remove the paragraph with class `pages-access-note` from `index.html` and commit that edit.

Applicants sign in with ChatGPT for this existing form. The backend is hosted by ChatGPT Sites; its availability and pricing are separate from GitHub Pages. If you want to remove this dependency, the form needs a separate backend and an authentication migration before switching its links. GitHub Pages alone cannot replace it. Do not publish secret keys or personal application data in a GitHub repository.

Joining the WhatsApp group remains available independently and does not mean acceptance as an official club member.

## What to edit

- `index.html`: page copy, recruitment link, administration link and opening notice.
- `styles.css`, `recruitment.css`, `pages.css`: appearance.
- `app.js`: interactions and exact seven-member order.
- `scene.js`: 3D camera.
- `recruitment.js`: interest explorer; no submission API.
- `assets/`: club imagery and local fonts.
- `vendor/`: self-hosted Three.js.

The original server-backed Site has not been changed by this export. Keep that project as the source of the working database and administration system.

## Validation

Before handoff: local link/asset resolution, script syntax, exact team order, multi-interest interaction, absence of local API calls, social URLs and original image hashes are checked. Browser-rendered visual appearance and GPU performance have not been rechecked in this session. GitHub deployment is not complete until Pages reports success in your repository.

## Credits and documentation

Original club photographs and characters remain unchanged. Three.js license: `vendor/THREE-LICENSE.txt`. Font licenses: `assets/FONT-LICENSES.txt`.

- GitHub Pages setup: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- Branch publishing settings: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
