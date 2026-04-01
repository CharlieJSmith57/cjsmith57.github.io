# Mechanical Engineering Portfolio

A dark, sleek personal portfolio site built for GitHub Pages. No frameworks, no build tools — just HTML, CSS, and vanilla JS.

## File Structure

```
portfolio/
├── index.html          ← Home / intro page
├── projects.html       ← All projects listing
├── project-1.html      ← Lightweight Structural Chassis
├── project-2.html      ← Heat Exchanger Optimization
├── project-3.html      ← 6-DOF Robotic Gripper
├── about.html          ← About / CV page
├── _config.yml         ← GitHub Pages config
└── assets/
    ├── style.css       ← All styles
    ├── main.js         ← Nav + scroll animations
    └── resume.pdf      ← (add your resume here)
```

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g. `your-username.github.io` for a root site, or any name for a project site)
2. Upload all files in this folder to the repository
3. Go to **Settings → Pages**
4. Under "Source", select **Deploy from a branch**
5. Choose `main` branch and `/ (root)` folder
6. Click Save — your site will be live at `https://your-username.github.io` within a few minutes

## Customizing

### Personal info
Search and replace these placeholders across all files:
- `Your Name` → your real name
- `YN` → your initials (avatar on About page)
- `your@email.com` → your email
- `ME.` → your initials logo (top left nav)
- LinkedIn / GitHub links → your actual URLs

### Projects
Each project page (`project-1.html`, etc.) has clearly labeled sections:
- Edit the `<h1>` for the project name
- Edit the `.project-meta` items for year/role/duration/industry
- Edit the `.project-tags` for your actual tools
- Edit the sidebar lists for tools, processes, standards
- Edit the result grid numbers
- Edit the `<article>` body text with your real project description

To add a new project:
1. Duplicate `project-3.html` → `project-4.html`
2. Add a card for it in `projects.html` and `index.html`
3. Update the "Next/Previous Project" nav links

### Photos / images
Replace the gradient `.project-cover` divs with real `<img>` tags:
```html
<div class="project-cover">
  <img src="assets/images/project-1-cover.jpg" alt="Chassis render" style="width:100%; height:100%; object-fit:cover;">
</div>
```

### Accent color
The lime-green accent (`#c8ff00`) is defined as `--accent` in `assets/style.css`.
Change it to any color you like — one edit updates the whole site.

### Resume
Drop your PDF at `assets/resume.pdf` — it's already linked from the About page and the contact section.

## Fonts
Uses Google Fonts (loaded via CDN):
- **Bebas Neue** — display headings
- **DM Sans** — body text
- **DM Mono** — labels, tags, meta

All fonts load from `fonts.googleapis.com` — works fine on GitHub Pages.
