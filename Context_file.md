# Sajal Debnath — Personal Website

Academic and professional portfolio site for **Sajal Debnath**, hosted on GitHub Pages.

**Live URL:** [https://sajaldeb25.github.io/sajal-debnath/](https://sajaldeb25.github.io/sajal-debnath/)

---

## Purpose

This is a single-page portfolio website that presents Sajal's research background, publications, professional experience, skills, and contact information. It serves as a public-facing profile for:

- Research collaboration inquiries
- Full-time job opportunities
- Academic and professional networking

The site is designed for recruiters, collaborators, and peers in AI/ML, healthcare analytics, and software engineering.

---

## About the Owner

**Sajal Debnath** is a Researcher & Software Engineer specializing in:

- Artificial Intelligence (AI) and Machine Learning (ML)
- Healthcare Analytics
- Streaming data analysis and fuzzy systems
- Multi-objective optimization

He holds a B.Sc. in Computer Science and Engineering from the University of Barishal (2022, CGPA 3.73/4.00) and works as a Software Engineer at Brain Station-23 PLC, Bangladesh.

Research areas include Alzheimer's disease detection, cancer chemotherapy scheduling, adaptive fuzzy classifiers, and interdisciplinary quantum-DNA computing projects.

---

## Site Structure

The website is a **single-page application** (`index.html`) with anchor-linked sections:

| Section | ID | Content |
|---------|-----|---------|
| Home | `#top` | Bio, tagline, profile photo |
| News | `#news` | Year-tabbed timeline (2025, 2024, 2023–Past) |
| Education | `#education` | Academic degrees and thesis |
| Publications | `#publications` | Published papers and under-review work |
| Experience | `#experience` | Professional roles with timeline layout |
| Skills | `#skills` | Programming, software, soft skills, languages |
| Achievements | `#problem-solving` | Competitive programming, certifications |
| Contact | `#contact` | Email, GitHub, LinkedIn, Facebook, Google Scholar |

Additional links:

- **CV** — Google Drive PDF (opens in new tab)

---

## Design

The site uses the **Modern Professional** visual theme:

- **Font:** Plus Jakarta Sans (Google Fonts)
- **Light theme:** Light gray background, white elevated cards, indigo + teal accents
- **Dark theme:** Slate background, darker cards, lighter indigo/teal accents
- **Layout:** Fixed left sidebar navigation + scrollable main content area
- **Hero:** Gradient background, rounded profile photo frame
- **Components:** Pill-style news tabs, publication badges, skill chips, experience timeline, circular contact icons

### Color palette (light mode)

| Role | Color |
|------|-------|
| Background | `#f0f2f5` |
| Surface / cards | `#ffffff` |
| Primary accent | `#4f46e5` (indigo) |
| Secondary accent | `#0d9488` (teal) |
| Text | `#1e293b` |

---

## Features

### Left sidebar navigation
- Fixed sidebar with links to all main sections
- Scroll-spy highlights the active section while scrolling
- Collapsible on desktop — collapses to a narrow strip showing only the expand button
- Collapse state persisted in `localStorage`

### Dark / light theme
- Toggle at the bottom of the sidebar
- Preference saved in `localStorage`
- Applied before page render to avoid flash of wrong theme

### Mobile responsive
- Sidebar becomes a slide-in drawer with hamburger menu
- Backdrop overlay closes the menu on tap
- Full sidebar content shown on mobile regardless of desktop collapse state

### News tabs
- Three year groups: 2025, 2024, 2023–Past
- Pill-style tab buttons with active state styling

---

## Tech Stack

| Layer | Technology |
|-------|------------|
| Markup | HTML5 |
| Styling | Embedded CSS with CSS custom properties |
| Scripting | Vanilla JavaScript (no frameworks) |
| Fonts | Google Fonts (Plus Jakarta Sans) |
| Hosting | GitHub Pages |
| Assets | Local profile image (`sajal_debnath.jpg`) |

No build tools, bundlers, or npm dependencies are required.

---

## File Structure

```
My website/
├── index.html          # Complete site (HTML + CSS + JS)
├── sajal_debnath.jpg   # Profile photo (required for hero section)
└── README.md           # This file
```

---

## Deployment

The site is published via **GitHub Pages** from the repository:

**Repository:** `Sajaldeb25/sajal-debnath` (or equivalent GitHub user/org repo)

To deploy updates:

1. Edit `index.html` locally
2. Ensure `sajal_debnath.jpg` is in the same directory
3. Commit and push to the GitHub repository
4. GitHub Pages serves the site at the URL above (may take 1–2 minutes to update)

---

## Key External Links

| Label | URL |
|-------|-----|
| CV | [Google Drive](https://drive.google.com/file/d/1M0lQ2R4tjtMPH4pTIB2f_6ft4eR_jUaX/view?usp=sharing) |
| GitHub | [github.com/Sajaldeb25](https://github.com/Sajaldeb25) |
| LinkedIn | [linkedin.com/in/sajal-debnath-6ab44b16b](https://www.linkedin.com/in/sajal-debnath-6ab44b16b/) |
| Google Scholar | [scholar.google.com](https://scholar.google.com/citations?hl=en&user=Zi30rKgAAAAJ) |
| Email | sajal.cse3.bu@gmail.com |

---

## Browser Storage

The site uses `localStorage` for two preferences:

| Key | Values | Purpose |
|-----|--------|---------|
| `theme` | `"light"` / `"dark"` | Color theme |
| `sidebarCollapsed` | `"true"` / `"false"` | Sidebar collapse state (desktop) |

---

## Maintenance Notes

- **Content updates:** Edit the relevant section directly in `index.html`
- **New publication:** Add a `<li>` entry under Publications → Published Papers
- **News item:** Add a `<div class="news-item">` block in the appropriate year tab
- **Meta tags:** Update `<meta name="description">` and Open Graph tags in `<head>` if the tagline or focus changes
- **Copyright:** Update the year in the Contact section footer as needed

---

## Version History

| Date | Change |
|------|--------|
| 2026 | Modern Professional redesign — left sidebar, dark/light theme, collapsible menu, skill chips, experience timeline |
| Earlier | Original top-navbar layout with card sections |
