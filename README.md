# The Commonplace

A small static site. No build step, no dependencies — just open `index.html`.

## Files
- `index.html` — the home page (masthead, Written, Made)
- `would-it-still-be-me.html`, `palantir-moat.html` — the essay reading pages
- `style.css` — all styling (edit the `--accent` variable at the top to change the mood)
- `*.md` — the source text for each essay, kept for reference

## To publish
Drop the folder on GitHub Pages, Vercel, or Cloudflare Pages. It's plain HTML/CSS.

## Still to fill in
- Footer links: email, GitHub, LinkedIn (currently placeholders)
- The Ambit "View →" link (currently `#`)
- Real dates on essays if you want day-level precision (currently "September 2026")

## Adding a new essay
1. Write it, save the `.md`.
2. Copy an existing essay `.html`, swap in the new title, date, and prose.
3. Add an `<a class="entry">` block to the "Written" section of `index.html`.

## More animation later
The scroll-reveal is a small dependency-free script at the bottom of each page.
For finer control (staggers, timelines, scroll-scrubbing), swap in GSAP + ScrollTrigger.
