# Personal Portfolio Template

A minimal personal portfolio template built with plain HTML and CSS. No frameworks, no npm, no build step — just open the file and start editing.

**Sections:** Hero (name, photo, bio) · Projects (3 cards) · Contact & Links

---

## Prerequisites

Before you start, make sure you have these installed:

- [Git](https://git-scm.com) — for version control and pushing your code
- [VS Code](https://code.visualstudio.com) — code editor (recommended)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) — VS Code extension that auto-refreshes your browser on save
- A [GitHub](https://github.com) account — to host your code
- A [Vercel](https://vercel.com) account (sign up with GitHub) — to deploy your site

---

## Step 1: Get the template

Open your terminal and run:

```bash
git clone [this-repo-url] my-portfolio
cd my-portfolio
```

Then open the folder in VS Code:

```bash
code .
```

---

## Step 2: Run it locally

Right-click `index.html` in the VS Code file explorer → **Open with Live Server**.

Your portfolio will open at `http://127.0.0.1:5500`. Any time you save a file, the browser refreshes automatically.

> No Live Server? Just double-click `index.html` to open it in your browser. Refresh manually after each change.

---

## Step 3: Make it yours

Search for every `TODO` comment in the files — they tell you exactly what to change.

### `index.html`

| What to change | Where to find it |
|---|---|
| Page title | `<title>` tag in `<head>` |
| Your photo | Replace `photo.jpg` with your own image file (same name) |
| Your name | `<h1 class="hero-name">` |
| Your role / tagline | `<p class="hero-title">` |
| Your bio | `<p class="hero-bio">` |
| GitHub profile URL | Both `<a>` tags with `href="#"` near GitHub |
| LinkedIn profile URL | Both `<a>` tags with `href="#"` near LinkedIn |
| 3 project names | `<h3 class="project-name">` in each card |
| 3 project descriptions | `<p class="project-description">` in each card |
| 3 project repo URLs | `<a href="#">` in each card |
| Your email | `<a href="mailto:...">` in the contact section |
| Copyright name | `<p class="copyright">` |

### Adding your photo

1. Find a photo of yourself (a headshot works best)
2. Rename the file to `photo.jpg`
3. Drop it into the `my-portfolio` folder (same level as `index.html`)
4. The image will appear automatically — no code changes needed

### `style.css`

Open `style.css` and look at the `:root` block at the very top:

```css
:root {
  --color-accent: #0057ff;   /* TODO: Change to your favorite color */
  ...
}
```

Change `--color-accent` to any hex color and it updates buttons and links everywhere at once. That's the only thing you need to touch to make it feel like yours.

---

## Step 4: Save your changes to GitHub

```bash
# Initialize a new git repo (skip if you already cloned this)
git init

# Stage all your changes
git add .

# Commit with a message
git commit -m "Initial commit: my portfolio"
```

Then go to [github.com](https://github.com), click **New repository**, give it a name (e.g. `my-portfolio`), and **do NOT** initialize with a README or .gitignore.

Copy the repo URL and run:

```bash
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git branch -M main
git push -u origin main
```

---

## Step 5: Deploy to Vercel

1. Go to [vercel.com](https://vercel.com) and log in with GitHub
2. Click **Add New... → Project**
3. Find your repository and click **Import**
4. Leave all settings as-is and click **Deploy**
5. In about 30 seconds, Vercel gives you a live URL — share it!

Every time you push a new commit to GitHub, Vercel automatically redeploys.

---

## Troubleshooting

**My photo isn't showing.**
Make sure the file is named exactly `photo.jpg` (lowercase, `.jpg` extension) and is in the same folder as `index.html`.

**My code isn't pushing to GitHub.**
Run `git remote -v` to check the remote URL. If it's wrong, update it:
```bash
git remote set-url origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
```

**Vercel deployment failed.**
Click the failed deployment in the Vercel dashboard and check the build logs. For a plain HTML site there's almost nothing to go wrong — the most common cause is the repo being empty or `index.html` not being at the root of the folder.

**I want to add more projects.**
Copy one of the `<!-- PROJECT -->` card blocks in `index.html` and paste it inside `.projects-grid`. Update the content and you're done.

---

## File structure

```
my-portfolio/
├── index.html    # All the content — edit this
├── style.css     # All the styles — edit the :root variables at the top
├── photo.jpg     # Your photo — add this yourself
└── README.md     # This file
```
