# Muhammad Hasnain Khan: Developer Portfolio

A responsive, dark-themed personal portfolio built with plain HTML, CSS and JavaScript.
No build step, no framework, no backend and no paid services, so it loads fast and deploys anywhere static files can be hosted.

## Folder structure

```
portfolio/
├── index.html          # All page content and sections
├── css/
│   └── styles.css      # Design tokens, layout, components, responsive rules
├── js/
│   └── main.js         # Mobile menu, active nav link, scroll reveal
├── assets/
│   └── favicon.svg     # Site icon
├── .nojekyll           # Tells GitHub Pages to serve files as-is
└── README.md
```

## 1. Run it locally in VS Code

**Option A: Live Server (recommended)**

1. Install [VS Code](https://code.visualstudio.com/).
2. Open the `portfolio` folder: **File → Open Folder...**
3. Open the Extensions panel (`Ctrl+Shift+X`), search for **Live Server** (by Ritwick Dey) and install it.
4. Right-click `index.html` and choose **Open with Live Server**.
5. Your browser opens the site and reloads automatically when you save a file.

**Option B: no extension needed**

Open the VS Code terminal (`Ctrl+` ` ``) in the `portfolio` folder and run:

```bash
python -m http.server 8000
```

Then visit <http://localhost:8000>. (On some systems the command is `python3`.) Press `Ctrl+C` to stop.

**Option C:** double-click `index.html`. It works directly from the file system too.

## 2. Upload it to GitHub

1. Sign in at <https://github.com> and click **New repository**.
2. Name it. For the simplest URL, use exactly `hasnain09july-a11y.github.io` (see the Pages section below). Choose **Public**. Do not add a README, .gitignore or license (you already have files).
3. In the VS Code terminal, inside the `portfolio` folder, run:

```bash
git init
git add .
git commit -m "Add portfolio website"
git branch -M main
git remote add origin https://github.com/hasnain09july-a11y/hasnain09july-a11y.github.io.git
git push -u origin main
```

If you named the repository something else, replace the URL in the `git remote add` line with your repository's URL (GitHub shows it on the empty repository page).

If Git asks you to sign in, follow the browser prompt, or use a personal access token as the password.

To publish later changes:

```bash
git add .
git commit -m "Describe your change"
git push
```

## 3. Publish with GitHub Pages

1. Open your repository on GitHub and go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Under **Branch**, select `main` and the `/ (root)` folder, then click **Save**.
4. Wait one to two minutes, then refresh the Pages settings. A banner shows your live URL:
   - If the repository is named `hasnain09july-a11y.github.io`: `https://hasnain09july-a11y.github.io/`
   - For any other repository name: `https://hasnain09july-a11y.github.io/<repository-name>/`

All file paths in the site are relative, so it works at either kind of URL without changes.

## Editing content

- **Text, projects, links:** edit `index.html`. Each section is marked with a comment such as `<!-- PROJECTS -->`.
- **Colors and spacing:** edit the variables in the `:root` block at the top of `css/styles.css`.
- **Adding a project:** copy one `<article class="project-card ...">` block inside the Projects section and update the text and GitHub link.

## Checklist before sharing

- [ ] Open every nav link and both buttons in the hero.
- [ ] Click both "View on GitHub" buttons and the GitHub and LinkedIn cards.
- [ ] Confirm the email link opens your mail app.
- [ ] Resize the browser narrow to check the mobile menu.
