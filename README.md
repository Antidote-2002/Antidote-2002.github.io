# Antariksha Jana — Personal Portfolio & SSD HTML/CSS Coursework

This repository contains my personal GitHub Pages portfolio and the styled SSD course page created for the HTML/CSS coursework.

## Live Pages

- **Personal portfolio:** https://Antidote-2002.github.io/
- **Styled SSD course page:** https://Antidote-2002.github.io/ssdcoursepage.html

The submission URLs are also stored in `2026202018_htcs.txt`.

---

## Personal Portfolio

The main page is `index.html`, styled by `style.css`.

The portfolio presents my academic journey from **B.E. in Civil Engineering at Jadavpur University** to **M.Tech in CSIS at IIIT Hyderabad**, along with my academic achievements, technical interests, skills and hobbies.

### Main features

- Responsive crimson/red visual theme
- Animated and interactive CSS effects
- About and academic journey sections
- Education section with alma-mater photographs
- Academic achievements
- Technical skills and current areas of exploration
- Hobbies and interests:
  - Gaming — FIFA and Call of Duty
  - Watching chess
  - Occasional table tennis
  - Watching football
  - Sketching
- Clickable GitHub and LinkedIn links
- Private contact form powered by Formspree
- Custom `AJ` favicon for the browser tab
- Responsive layouts for desktop and mobile
- Reduced-motion support for users who prefer less animation

### Contact privacy

The public page does **not** display my personal email address.

Visitors can contact me through the Formspree form in `index.html`. The form collects the visitor's name, email, subject and message so I can reply without publishing my own email address on the website.

GitHub and LinkedIn remain directly accessible from the site.

---

## Education Images

The Education section currently uses:

- **IIIT Hyderabad** — Wikimedia Commons image loaded externally
- **Jadavpur University** — Wikimedia Commons image loaded externally
- **Ramakrishna Mission Vidyabhavan, Midnapore** — stored locally as `assets/images/rkmv-campus.jpeg`
- **Profile photo** — stored locally as `assets/images/profile.jpeg`

The site no longer contains a personal photo gallery.

Generic hobby images are loaded from Unsplash and are used only as visual illustrations of the hobbies.

Image attribution information is kept in `IMAGE_CREDITS.md`.

---

## SSD Course Page

`ssdcoursepage.html` contains the styled version of the **CS6.302 — Software System Development, Monsoon 2026** course page.

The original course-page structure and content are retained, while additional styling is loaded through:

```css
@import url("ssd-extra.css");
```

`ssd-extra.css` adds:

- red-accented visual styling
- improved typography and spacing
- card-like table presentation
- styled navigation links
- gradients and shadows
- hover effects
- responsive layouts
- improved mobile readability
- CSS pseudo-elements and attribute selectors

The SSD page remains separate from the personal portfolio so it can be opened directly at:

```text
https://Antidote-2002.github.io/ssdcoursepage.html
```

---

## Repository Structure

```text
Antidote-2002.github.io/
├── index.html
├── style.css
├── ssdcoursepage.html
├── ssd-extra.css
├── 2026202018_htcs.txt
├── IMAGE_CREDITS.md
├── README.md
├── favicon.svg
├── favicon.ico
├── favicon-32x32.png
├── apple-touch-icon.png
└── assets/
    └── images/
        ├── profile.jpeg
        └── rkmv-campus.jpeg
```

---

## Technology Used

- HTML5
- CSS3
- CSS Grid
- Flexbox
- Responsive media queries
- CSS animations and transitions
- Pseudo-elements
- Formspree for the private contact form
- Git and GitHub
- GitHub Pages

The portfolio is intentionally lightweight and does not require a JavaScript framework or build system.

---

## Running Locally

Clone the repository or open the project directory and run:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000/
http://localhost:8000/ssdcoursepage.html
```

Stop the server with:

```text
Ctrl+C
```

The pages can also be previewed using VS Code Live Server.

---

## GitHub Pages

The repository is published through GitHub Pages from the `main` branch.

Because the repository is named `Antidote-2002.github.io`, the root `index.html` is served as the personal homepage.

---

## Notes

- The résumé is intentionally not published in this repository.
- The personal email address is intentionally not written in the public website files.
- Only the main profile photo is used as a personal photograph.
- The Ramakrishna Mission campus photo is stored locally so it does not depend on a third-party image hotlink.
- `IMAGE_CREDITS.md` contains attribution/source information for the external images used by the project.
