# Vittoria Cugno portfolio

Portfolio site for Vittoria Cugno, an oil painter in Naarm/Melbourne.
Plain HTML and CSS, no build step: open the .html files in a browser to view them.

## Files

- index.html: work page, with a feature image and a grid of artworks
- about.html: about page, with bio, photo, contact links and CV
- exhibitions.html: one exhibition (Interior/Exterior), with text and an
  image slider that needs no JavaScript
- style.css: all the site's styles
- fonts/: the site's fonts
- js/ and css/: code from other people that the gallery uses (jQuery, Justified Gallery)
- Images are hosted on Cloudinary, not in this folder

## House rules

- Use the colour variables at the top of style.css (--primary-bg-colour,
  --darkbrown, --orange, --warmlightgrey) instead of typing new colour codes
- Use the spacing variables at the top of style.css (--space-xs, --space-s,
  --space-m, --space-l, --space-xl) instead of typing new spacing values.
  Use gap on the parent for even spacing (.stack for columns), and margin
  only for one-off exceptions. Don't add new margin classes like mt-50
- Use the fonts already set up in style.css: Sentient for headings,
  Kyneton Art Grotesque for body text, ChiffChaff for the logo,
  Roboto Mono for captions
- Put new styles in style.css, under the matching comment heading
- Style for phones first, then add changes for wider screens inside
  @media (min-width: 768px)
- Write site text in Australian English

## How I like to work

- I'm new to coding and to Claude Code, so go slowly: one step at a time,
  and explain what you're doing before you do it
- I'm learning from this project. When I ask how something works, or I'm
  building something I want to learn from, use the teach-me skill
  (.claude/skills/teach-me/). If I just want something done, do it
- Explain any new term once, in plain words
- Before changing a file, tell me what you'll change and why

## Memory

Notes carried between chats. Read these before starting work.

How to keep this up to date:
- At the end of a chat where something was decided, started or taught,
  add a short dated note here and tell me what you added
- Only note things the code doesn't show: decisions and why, unfinished
  work, lessons covered
- When I say "remember this", add it here
- Delete notes once they're finished or no longer true, and keep this
  section short

### Unfinished work

- 2026-10-17: Exhibitions slider still uses the demo travel photos.
  Replace each src with Vitt's images and write real alt text
- 2026-10-17: Slider arrows are centred on the tallest image, so they sit
  low on shorter ones. Possible fix: aspect-ratio on the slides
- 2026-10-17: Spacing cleanup done but not yet checked in a browser
- 2026-10-17: CV text for Vitt to check: "Red Stockrooom", "Echoes of a
  Gaze,</i>," (double comma), "Capture</i>,RMIT" (missing space), and
  "Art Almanac October 2025" listed twice

### Lessons covered

- 2026-10-16/17: Parent and child elements; flexbox and two-column
  layouts; mobile-first media queries; CSS Grid for rows; classes need a
  matching CSS rule; descendant selectors; specificity; the box model and
  box-sizing; SCSS versus CSS; position relative and absolute; transform
  replaces rather than adds; optical centring; gap only works on flex or
  grid parents; gap versus margin and spacing scales
