# farhanfuadabir.github.io

Personal site for Farhan Fuad Abir, live at <https://farhanfuadabir.github.io/>.

A single hand-written static page. No build step, no framework, no dependencies.

## Layout

```
index.html          home: about, now, updates, selected work
publications.html   the complete publication list
projects.html       research and hardware projects, written up
cv.html             CV as a web page, with the PDF linked
offline.html        teaching, community, competitions (not linked from home)
blog/               plain-language write-ups of papers (light, Google Research-style layout)
assets/style.css    every page except blog/ shares this one stylesheet
assets/blog.css     stylesheet for blog/
assets/img/blog/    figures used by blog posts
assets/cv.pdf       CV PDF, linked from the header and cv.html
assets/img/         profile photo
.nojekyll           serve raw HTML instead of running Jekyll
robots.txt
sitemap.xml
```

## Editing

Open the page you want and edit it. Content blocks are marked with HTML comments
(`<!-- INTRO -->`, `<!-- ABOUT -->`, `<!-- NOW -->`, `<!-- UPDATES -->`,
`<!-- PUBLICATIONS -->`, `<!-- PROJECTS -->`, `<!-- CONTACT -->`).

### Adding an update

The `<!-- UPDATES -->` block on `index.html` carries a comment with a copy-paste
template. Newest goes on top:

```html
<div class="update">
  <div class="ud">Mon YYYY</div>
  <div class="ub">What happened, in a sentence or two.</div>
</div>
```

Add `class="update pin"` to print the date in claret for something you want to stand out.

### Styling

All styles live in `assets/style.css`, shared by all five pages. Change a color once
in the `:root` block at the top and every page follows.

Preview locally:

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Deploy

Push to `main`. GitHub Pages serves this user repo from `main` at the repo root;
the live site refreshes about a minute later.

## Design

Dark mid-tone only. Graphite ground `#3B3B39`, bone text `#F4F1EA`, a single ochre accent
`#E2A93B` (hover `#F0C069`). Type is Spectral (headings), Karla (body), and Red Hat Mono
(labels and meta), loaded from Google Fonts. One ~660px column, generous whitespace,
hairline dividers.

The previous al-folio Jekyll version of this site remains in the git history.
