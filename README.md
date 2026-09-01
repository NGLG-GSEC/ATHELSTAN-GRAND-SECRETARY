# Grand Secretary — Masonic Order of Athelstan

The way in to the work of the Secretariat. This repository holds the menu;
each section of the work keeps its own repository, its own history and its own
site.

**https://dskiad.github.io/ATHELSTAN-GRAND-SECRETARY/**

> The link goes live once GitHub Pages is enabled for this repository:
> **Settings → Pages → Build and deployment → Source: _GitHub Actions_**.
> The workflow in `.github/workflows/pages.yml` publishes every push to `main`.

## The sections

| Section | Where it lives | Access |
| --- | --- | --- |
| Rosetta Stone, Volume 6 | [`dskiad/rosetta-stone-mo-athelstan-volume6`](https://github.com/dskiad/rosetta-stone-mo-athelstan-volume6) | private |
| Software of the Order | [`TechIns-Group-Software-Development`](https://github.com/TechIns-Group-Software-Development) — `rosetta_stone`, `b2b_v2` | private |
| Summonses & returns | here, in preparation | — |

A private repository opens only for a GitHub account that has been given
access, and has no public site. The cards say so.

## The two offices

This is one of two: the [Grand Chancellor](https://github.com/dskiad/Grand-Chancellor)
keeps the patents, certificates and recognition of the National Grand Lodge of
Greece. Each site carries a switch to the other in its top bar, and its own copy
of `assets/portal.css`, so neither depends on the other being up.

## Adding a section

A section that lives elsewhere is a card in `index.html`:

```html
<a class="doc-card away" href="https://github.com/owner/repo">
  <span class="tag private">Private</span>     <!-- or: <span class="tag">Ready</span> -->
  <h3>Its name</h3>
  <p>One sentence on what it is.</p>
  <span class="where">owner / repo</span>
</a>
```

`away` marks a card that leaves this site; drop it for a page held here. A
section still being built is a `<div class="doc-card soon">` with an
*In preparation* tag.

A section held **here** — a form of the Secretariat, say — works exactly like
the Chancellor's patents: copy `patents/past-grand-officer.html` and the
`assets/` folder from
[`dskiad/Grand-Chancellor`](https://github.com/dskiad/Grand-Chancellor), whose
README documents the engine.
