# Dr. Mohd Sakib — Academic Website

Personal academic website for Dr. Mohd Sakib, Assistant Professor, School of Computer Science,
UPES University, Dehradun, India.

**Live site:** https://sakib9286.github.io/

## What is here

```
index.html                     Single-page site (all content)
assets/css/style.css           Styles, light + dark themes
assets/js/main.js              Nav, filters, counters, theme toggle
assets/img/portrait.jpg        Profile photo
assets/img/og-cover.jpg        Link preview card for social/email
assets/files/Mohd_Sakib_CV.pdf Downloadable CV
```

No build step, no dependencies. It is plain HTML, CSS, and JavaScript, so GitHub Pages
serves it as is.

## How to update it

**Publications, awards, anything textual** — open `index.html` and edit the text.
Each publication is one `<li class="pub" data-cat="...">` block; copy an existing one
and change the fields. Valid `data-cat` values are `journal`, `conference`, `chapter`,
and `press` (in press or under review).

**Citation counts** — search `index.html` for `data-count` and update the numbers,
plus the "as of" line just below the stats.

**A new CV** — replace `assets/files/Mohd_Sakib_CV.pdf`, keeping the same file name.

**Photo** — replace `assets/img/portrait.jpg` with a square image, ideally 900x900.

After editing:

```bash
git add -A
git commit -m "Update publications"
git push
```

GitHub Pages redeploys within about a minute.

## Local preview

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000
