# Lorena G. Barberia: personal academic website

A plain HTML/CSS site (no build step) laid out like shirokuriwaki.com: a fixed bio sidebar on the left and the papers, teaching, and data on the right.

## Files
- `index.html`: all page content. Edit the text directly.
- `style.css`: layout and colours.
- `images/`: put `headshot.jpg` (square) and `banner.png` (a wide research figure) here.
- `cv/barberia_cv.pdf`: the CV the sidebar links to.

## Editing
- **Add a paper:** copy an existing `<li>...</li>` block in the right section and change the title, link, coauthors, and venue. The `<details>` block (the abstract) and the `Copy BibTeX` button with its `<template>` are optional.
- **Draft markers:** text tagged `<span class="todo">...</span>` shows as a yellow label. Fill in the content, then delete the span.
- **Photo / banner:** in `index.html`, change `images/headshot.svg` to `images/headshot.jpg`, and replace the `banner-placeholder` div with `<img src="images/banner.png" alt="...">`.

## Preview locally
```
python3 -m http.server 8080   # then open http://localhost:8080
```

## Publish free on GitHub Pages
1. Create a public repo called `lorena-barberia.github.io` and push these files to it.
2. In the repo, go to Settings > Pages and choose "Deploy from branch: main / root".
3. The site goes live at https://lorena-barberia.github.io. To use a custom domain, add it under the same settings page.
