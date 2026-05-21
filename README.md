sticker bomb template

a composition notebook-style collection page for stamps, stickers, gifs, buttons, blinkies, userboxes, and trinkets. items are randomly placed in a grid with rotation and overlap, mimicking a sticker-bombed notebook cover.

## how to customize

1. **images** — edit the `stamps`, `stickers`, `gifs`, `buttons`, `blinkies`, `userboxes`, and `trinkets` arrays in the `<script>` section. replace the placeholder urls with your own image paths.

2. **colors** — edit the `:root` variables in `<style>`. palette covers background, surface, text, accent, label, ruler lines, and shadows.

3. **background** — replace `compnotebookbg.jpg` with your own background image, or remove the `background-image` line to use just the solid `--bg` color.

4. **label text** — edit the text inside `.comp-label-title` and `.comp-label-sub`.

5. **nav link** — change the `<a>` href and text to point to your home page.

6. **sizes** — adjust the config variables (`STAMP_SIZE`, `CELL_SIZE`, `ROTATION_MAX`, `JITTER`, etc.) to control item density and spacing.

7. **adding new categories** — push objects with `{ src, type }` into `allItems`, add a type check in the placement logic, and add a corresponding css class.

## key sections

- `:root` — color palette
- `.collections-page` — page layout + background
- `.comp-label` — fixed top label with ruled lines
- `stamp`, `sticker`, `gif`, etc. arrays — item data sources
- config vars — layout tuning constants
- resize handler — re-renders on window resize

## limitations

- designed for a single-page collection view; not a multi-page system
- uses `position: absolute` for item placement, so no document flow for items
- resize re-shuffles items; positions change on every window resize
- placeholder images use placehold.co; replace with your own assets for production
- requires javascript enabled

## license / usage

template by enargeia  
attribution: https://ko-fi.com/melanmel  
usage subject to distribution terms in repo/listing  
no redistribution or resale without permission
