# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

People evaluating **sh1ft3r** (the owner's developer identity) — recruiters, prospective clients, and peers who arrive from a link, a GitHub profile, or a search, and want to judge quickly whether this person is worth contacting. They are skimming, often on a phone, and usually comparing against several other developers in the same sitting.

Today the repository serves a second, incidental audience: developers who find the animated-title effect and read the source to learn how it works. This audience is not the one future work optimizes for.

## Product Purpose

The repository currently holds a single-page CSS demo: three words that crossfade with a gradient clipped to the glyphs. Its confirmed destination is to become **sh1ft3r's personal site and portfolio**, with the animated title as the seed of that surface rather than the whole of it.

Success is a visitor leaving with an accurate, favorable impression of the owner's craft, and knowing how to reach them.

## Positioning

**Open — not yet decided.** No differentiating claim has been established. The only asset with a claim attached today is the execution quality of the animation itself. Future work must not invent a specialty, a years-of-experience figure, a client roster, or a niche; those are the owner's to declare.

## Operating Context

- The site is opened directly from the filesystem or from a static host. There is no server, no session, and no state.
- Visitors are unauthenticated strangers arriving cold, with no prior context about the owner.
- The repository lives at `github.com/carlosAndress101/Title-animate` on GitHub, `master` branch. No deploy target has been confirmed.

## Capabilities and Constraints

**Confirmed and binding:**

- **Zero dependencies, no build step.** Plain HTML and CSS that runs when `index.html` is opened in a browser. No npm, no bundler, no framework. This is a durable constraint the owner locked deliberately — it survives redesigns and the growth into a full site.

**Explicitly open (do not treat as fixed):**

- The copy "Develop. Preview. Ship." is placeholder. It is Vercel's tagline, borrowed for the demo, and is expected to be replaced once the site has a real purpose. It carries no meaning about this product.
- The gradient-crossfade technique is not a commitment. It may be kept, evolved, or replaced.
- What the portfolio actually contains — work samples, writing, about, contact — is undecided.
- Deploy target is undecided.

**Current implementation facts:** the animation is one 8s keyframe shared by all three words, staggered by a per-element `--delay`; each word's text is duplicated between the element's text node and a `--content` custom property that `::before` renders as the gradient overlay. Type is a fixed `8rem`, which is not yet responsive.

## Brand Commitments

- **sh1ft3r** is the owner's handle and personal brand, and is binding. Future work should treat it as the identity of the site, not decoration.
- `image/sh1ft3r-logo.svg` is the master brand mark: an S drawn as two tangent elliptical arcs on a
  black rounded container, filled with the #007CF0 → #00DFD8 gradient the site's first line uses. Every
  raster form is generated from it, so the SVG is the one file to edit.
- `image/sh1ft3r-logo.ico` (16/32/48) and `image/apple-touch-icon.png` (180, opaque, square) are derived
  outputs. There is still no wordmark, no horizontal lockup, and no monochrome variant.
- No confirmed voice, tone, color, or typographic commitments beyond the handle and the mark.

## Evidence on Hand

- `index.html` / `style.css` — the animated title, the only real artifact.
- `image/sh1ft3r-logo.ico` — the brand mark, favicon-resolution only.
- `README.md` — two demo GIFs hosted on GitHub user-content; no prose.

**Absences future work must not fill by invention:** there are no work samples, no case studies, no bio, no testimonials, no clients, no metrics, no résumé, and no contact details anywhere in this repository. A portfolio built here needs the owner to supply that content; placeholder lorem or fabricated credentials would defeat the surface's only purpose.

## Product Principles

1. **The visitor is comparing, not browsing.** They are looking at several developers today. Whatever earns the first three seconds is the design problem.
2. **Craft is the argument.** With no client list or metrics to cite, the quality of the execution is the evidence. Anything sloppy on this surface is a counter-argument against its own thesis.
3. **The constraint is the point.** Dependency-free static is a deliberate limit, not a stage the project will grow out of. Ambition must be expressed within it.
4. **Nothing about the owner gets invented.** Every factual claim on this site comes from the owner. Absent content stays absent until supplied.
5. **The demo is a seed, not the ceiling.** The current page is one effect. It should not constrain what the eventual site becomes.
