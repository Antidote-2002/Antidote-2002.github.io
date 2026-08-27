# SSD HTML/CSS Practice Work — Final Project

This repository is ready to publish as the GitHub Pages site for **Antidote-2002**.

## Final structure

```text
Antidote-2002.github.io/
├── index.html
├── style.css
├── ssdcoursepage.html
├── ssd-extra.css
├── 2026202018_htcs.txt
├── README.md
└── assets/
    └── images/
        ├── profile.jpg
        ├── gallery-1.jpg
        ├── gallery-2.jpg
        └── gallery-3.jpg
```

The résumé PDF is intentionally **not** included in this website.

## What is included

### Personal page — `index.html`

- About
- Education
- Academic achievements
- Skills
- Academic focus
- Interests & hobbies
- Picture gallery
- Contact/GitHub information
- Responsive design for desktop and mobile

Important personal-site choices:

- GATE CS AIR 994 is given highest priority among the 2026 exam achievements.
- Programming skills are **C++, Python and SQL**. C is not listed.
- No work experience has been invented. The page uses an Academic Focus section instead.
- No résumé PDF is published.

### SSD page — `ssdcoursepage.html`

The page keeps the SSD course's table-based structure, section IDs and course content, while loading the extra styling through the original `<style>` area:

```css
@import url("ssd-extra.css");
```

The extra stylesheet demonstrates:

- element selectors
- class selectors
- ID selectors
- child/descendant selectors
- attribute selectors
- `:hover`
- `:nth-child()`
- `::before` / `::after`
- responsive media queries
- gradients, shadows and modern spacing

## 1. Replace the images

All four image files currently contain placeholders. You only need to overwrite them; **do not change their filenames**.

### Profile photo

Put your profile photo here:

```text
assets/images/profile.jpg
```

A portrait crop (roughly 4:5) works best.

Example:

```bash
cp ~/Pictures/my-profile.jpg assets/images/profile.jpg
```

### Gallery images

Overwrite:

```text
assets/images/gallery-1.jpg
assets/images/gallery-2.jpg
assets/images/gallery-3.jpg
```

Example:

```bash
cp ~/Pictures/campus.jpg assets/images/gallery-1.jpg
cp ~/Pictures/photo2.jpg assets/images/gallery-2.jpg
cp ~/Pictures/photo3.jpg assets/images/gallery-3.jpg
```

Linux filenames are case-sensitive, so `profile.jpg` and `Profile.jpg` are different files.

## 2. Optional LinkedIn link

The résumé names the LinkedIn profile but does not provide the exact profile URL, so the site does not publish an incorrect link.

If you want LinkedIn on the page, open `index.html`, find this comment:

```html
<!-- Add your exact LinkedIn profile URL here later if you want it public. -->
```

and add your exact link next to the GitHub/email links.

## 3. Run locally

From this directory:

```bash
firefox index.html
```

SSD page:

```bash
firefox ssdcoursepage.html
```

A better local test is:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/
http://localhost:8000/ssdcoursepage.html
```

Stop the server with `Ctrl+C`.

## 4. Create the GitHub repository

On the **Antidote-2002** account, create a public repository named exactly:

```text
Antidote-2002.github.io
```

If this project folder is on your Desktop:

```bash
cd ~/Desktop/Antidote-2002.github.io
```

Initialize Git:

```bash
git init
git branch -M main
git remote add origin https://github.com/Antidote-2002/Antidote-2002.github.io.git
```

Then:

```bash
git add .
git commit -m "Create personal page and styled SSD course page"
git push -u origin main
```

## 5. Enable GitHub Pages

Repository → **Settings → Pages**

Choose:

```text
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

Save.

## 6. Final URLs

```text
https://Antidote-2002.github.io/
https://Antidote-2002.github.io/ssdcoursepage.html
```

These URLs are already written in `2026202018_htcs.txt`.

## 7. Final checks

Before submission:

- replace all placeholder pictures
- open both pages locally
- push every file to GitHub
- confirm both URLs open in a private/incognito window
- confirm `2026202018_htcs.txt` has the two correct URLs
- confirm the résumé PDF is not present anywhere in the repository
- confirm the personal site lists C++, Python and SQL, not C
- confirm GATE appears first in the achievements section


## Personal narrative used in this version

The portfolio now highlights the academic transition from a B.E. in Civil Engineering at
Jadavpur University to an M.Tech in CSIS at IIIT Hyderabad, along with the 2026 GATE/ISI/PGEE
milestones. The visual design uses only HTML and CSS, including CSS Grid/Flexbox, gradients,
pseudo-elements, hover states, keyframe animation and responsive media queries.


## Final visual update

- Main visual accent changed to crimson/red.
- Personal gallery removed; only `assets/images/profile.jpg` remains as a personal photo.
- Education is presented with alma-mater imagery for:
  - IIIT Hyderabad
  - Jadavpur University
  - Ramakrishna Mission Vidyabhavan, Midnapore
- Image credits are documented in `IMAGE_CREDITS.md`.
- The SSD course-page redesign also uses the red-accent palette.

The alma-mater photos are externally hosted, so they load when the site has an internet connection
(which GitHub Pages normally does).


## Funky red design layer

The final portfolio keeps the crimson/red accent but adds:
- playful card tilts and hover motion
- moving gradient text
- subtle dotted page texture
- sticker-like labels
- floating/doodled decorative elements
- stronger interactive contact cards
- animated micro-details with reduced-motion support


## Private contact form setup

The portfolio intentionally contains **no owner email address** in its HTML, CSS or README.

The form uses Formspree's ID-based endpoint. Before publishing:

1. Create/log in to a Formspree account.
2. Create a new form and set its destination/target email privately in Formspree.
3. Open `index.html` and replace:

   `https://formspree.io/f/YOUR_FORM_ID`

   with the endpoint Formspree gives you, for example:

   `https://formspree.io/f/abcdwxyz`

Do **not** put your destination email address into the form action.

The visitor's email field uses `name="email"`, so Formspree can set that visitor as the Reply-To address.
A hidden `_gotcha` honeypot field is included for basic spam filtering.

### Privacy note

Removing an email from the current site files does not remove it from old Git commits if it was
published previously. If the repository has already been public with the email in older commits,
rewrite/remove that Git history separately if you want the old value to stop being recoverable from
the repository's history.


## Browser tab icon

The browser favicon matches the red `AJ` header mark.

Files:
- `favicon.svg` — primary modern favicon
- `favicon.ico` — browser compatibility fallback
- `favicon-32x32.png` — PNG fallback
- `apple-touch-icon.png` — home-screen/touch icon


## Hobbies & Interests section

The personal page now includes hobby cards for:
- Gaming — FIFA and Call of Duty
- Watching chess
- Occasional table tennis
- Watching football
- Sketching

The hobby images are generic Unsplash visuals, not personal photographs.
Their source pages are listed in `IMAGE_CREDITS.md`.
