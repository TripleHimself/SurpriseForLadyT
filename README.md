# Maybe It’s a Playlist. Maybe It’s a Letter.

Version 2 of a cinematic, responsive romantic playlist website with aurora gradients, twinkling stars, floating petals, animated chapter progress, typewriter text, scroll reveals, and interactive song cards. Chapter I is open and contains songs 1–20. Chapters II–V show their teaser text and remain locked.

## Publish on GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html`, `styles.css`, and `script.js` to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.

## Add the Spotify playlist

Open `script.js` and replace:

```js
const SPOTIFY_PLAYLIST_URL = "#";
```

with the public URL of your Spotify playlist.

## Reveal another chapter later

The current package intentionally includes only the 20 songs for Chapter I. To release a later chapter, add its 20 song objects to `SITE_DATA`, add the corresponding section/card rendering, and change that chapter’s `available` value to `true`. Keeping unreleased songs out of the public files prevents visitors from finding them early in the page source.

## Files

- `index.html`: page structure and metadata
- `styles.css`: responsive romantic design
- `script.js`: chapter data, songs, reveal interactions, and Spotify URL

No build process is needed. The website works as a normal static GitHub Pages site.

## Version 2 motion controls

The floating **ambience** button pauses or resumes decorative petals. Visitors who enable reduced motion in their device settings automatically receive a still, accessible version.

## Version 3 visual refinement

Version 3 replaces the original typography with **DM Serif Display** for romantic headings and **DM Sans** for comfortable reading. The introduction is deliberately smaller and left-aligned, while the burgundy, pink, coral, champagne, and ivory palette is brighter and more vibrant.

## Version 4 typography

Version 4 uses **Playfair Display** for romantic headings, chapter titles, quotations, and signature details, paired with **Inter** for the introduction, navigation, labels, and longer reading text. The intro remains deliberately compact for comfortable reading.

## Version 6 envelope chapters

The five chapter cards are styled as sealed envelopes with layered paper, triangular flaps, gold wax seals, lift animations, and distinct burgundy styling for the available first chapter.

Version 7 adds paper grain textures, wax-seal styling, subtler envelope motion, sans-serif song cards and removes decorative lyric quote marks.

Version 10 lowers the chapter availability labels below each envelope and gives the intro letter a blush, rose, champagne and textured stationery background.

## Version 11 refinements

Version 11 reduces expanded Feeling and Why text, removes both the Spotify music control and floating ambience control, keeps each weekly status on one line, and replaces the long Chapter I introduction with a compact romantic stationery panel showing the opening lines.

Version 11 fixed: removed a JavaScript reference to the deleted Spotify control that prevented scroll-reveal text from becoming visible.

## Version 12 chapter text

The Chapter I introduction now displays the complete long chapter text instead of only the first four paragraphs. Typography remains compact so the full passage fits naturally above the song tiles.

## Version 16 navigation

The intro letter now includes a prominent **Explore the Chapters** button that links directly to the chapter-envelope section using the existing smooth-scroll behavior.
