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
- **Planting densities**: spacing and plants per m² for every herbaceous and ground cover plant, with a table per guild showing how much ground they will cover.
- **Guild builder**: choose a centre tree and rootstock, add plants from each layer, and see the plan, planting densities, jobs covered (nitrogen fixing, nutrient mining, pollinators, pest control, ground cover, mulch), warnings, yield estimate and harvest calendar update live. Saved in the browser.
- **Sources**: linked further reading (Agroforestry Research Trust, Martin Crawford and Patrick Whitefield's books, UK forest garden studies, RHS fruit guides, Plants For A Future). Each tree's panel also links its RHS guide.
- **My guilds**: save guilds from the builder with a name, the year you planted them and notes. Each one shows its age and stage, this month's jobs (with tick boxes that reset monthly) and harvests across all your guilds, a month-by-month planner, a yearly upkeep list and an estimated harvest for this year. Saved in your browser; when the page is opened in Claude, guilds are stored privately to your account instead.
- **UK growing notes**: planting season, summer pruning of stone fruit, frost pockets, pollination groups, mulching and planning for shade.

## Editing the plants

All data lives in the `<script>` at the bottom of `index.html`:

- `PLANTS`: companion plants, with layer, jobs, harvest months and yield per plant (young / mature, kg).
- `SPACING`: planting density for herbaceous and ground cover plants (spacing in cm, plants per m², or sowing rate).
- `TREES`: centre trees, with rootstocks, calendars, pruning notes and the suggested guild.

Tree sizes, pruning times and pollination advice follow the RHS guides linked on the page. Yields are estimates from typical nursery figures, not guarantees.

## Hosting

Because it's one static file, GitHub Pages works: Settings → Pages → deploy from the branch root.
