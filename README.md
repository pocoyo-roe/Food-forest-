# The Guild Orchard

An interactive guide to growing a food forest in the UK, built around fruit tree guilds.

Open `index.html` in a browser. It is a single self-contained page with no build step.

## What's in it

- **Seven layers**: a cross-section of a mature apple guild. Hover or tap a layer to see what grows there.
- **Guild atlas**: nine UK fruit trees (apple, pear, plum, sweet cherry, damson, quince, medlar, black mulberry, fig). Each has:
  - a plan view of the guild, with every companion plant hoverable for details and why it's there
  - a calendar of blossom, harvest and pruning months, plus pruning notes
  - rootstock options and estimated yields for a young guild (years 3–4) and a mature guild (year 8+)
  - a whole-guild harvest calendar
- **Guild builder**: choose a centre tree and rootstock, add plants from each layer, and see the plan, jobs covered (nitrogen fixing, nutrient mining, pollinators, pest control, ground cover, mulch), warnings, yield estimate and harvest calendar update live. Saved in the browser.
- **UK growing notes**: planting season, summer pruning of stone fruit, frost pockets, pollination groups, mulching and planning for shade.

## Editing the plants

All data lives in the `<script>` at the bottom of `index.html`:

- `PLANTS`: companion plants, with layer, jobs, harvest months and yield per plant (young / mature, kg).
- `TREES`: centre trees, with rootstocks, calendars, pruning notes and the suggested guild.

Yields are typical ranges for UK gardens, not guarantees.

## Hosting

Because it's one static file, GitHub Pages works: Settings → Pages → deploy from the branch root.
