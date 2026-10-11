# The Guild Orchard

An interactive guide to growing a food forest in the UK, built around fruit tree guilds.

Open `index.html` in a browser. It is a single self-contained page with no build step.

## What's in it

Each main section opens and closes like a drop-down, so the page starts as a short list of headings. Nav links open the section they point to, "Open all sections" and "Close all" sit under the intro, and your choice is remembered.

- **Seven layers**: a cross-section of a mature apple guild. Hover or tap a layer to see what grows there.
- **Guild atlas**: an example guild for each of nine UK fruit trees (apple, pear, plum, sweet cherry, damson, quince, medlar, black mulberry, fig). Each has:
  - a plan or 3D view of the example guild, with every companion plant hoverable for details and why it's there, and a button to copy it into the builder
  - a calendar of blossom, harvest and pruning months, plus pruning notes
  - rootstock options and estimated yields for a young guild (years 3–4) and a mature guild (year 8+)
  - a whole-guild harvest calendar
- **Planting densities**: spacing and plants per m² for every herbaceous and ground cover plant, with a table per guild showing how much ground they will cover.
- **Guild builder**: switch between your saved guilds with the **Your guilds** drop-down (it asks before discarding unsaved changes, including a new guild you haven't saved yet; "Save it first" opens the save form and then carries on), choose a centre tree and rootstock, add plants from each layer, press **Edit layout** to move each plant to its own spot (drag it, or tap it and then tap where it should go; arrow keys nudge; distance and direction from the trunk are shown; **Reset to automatic layout** undoes it), and see the plan, planting densities, jobs covered (nitrogen fixing, nutrient mining, pollinators, pest control, ground cover, mulch), warnings, yield estimate and harvest calendar update live. Saved in the browser.
- **Sources**: linked further reading (Agroforestry Research Trust, Martin Crawford and Patrick Whitefield's books, UK forest garden studies, RHS fruit guides, Plants For A Future). Each tree's panel also links its RHS guide.
- **3D view** (in the builder, the guild atlas and My guilds): switch the plan to 3D to see the guild to scale, drag to turn it, jump to views from each side, above or at eye level, step through the months (bare branches, blossom, fruit, autumn colour) and compare a young guild with a mature one. Shadows follow the noon sun for each month. Uses three.js r128, loaded from cdnjs only when you open the 3D view.
- **My guilds**: save as many guilds as you like from the builder ("Start a new guild" or "+ Add another guild" begins a fresh one). View each guild on its own, or pick **All guilds** for combined jobs this month, a harvest calendar by crop, a month-by-month planner, merged upkeep, an overview of every plan and a 3D view of all guilds side by side. Save guilds with a name, the year you planted them and notes. Each one shows its age and stage, this month's jobs (with tick boxes that reset monthly) and harvests across all your guilds, a month-by-month planner, a yearly upkeep list and an estimated harvest for this year. Saved in your browser; when the page is opened in Claude, guilds are stored privately to your account instead.
- **Site plan** (My guilds → Whole garden → Site plan): set your plot's width and length, drag corners or add more for an irregular boundary, set which way is north, add buildings, sheds, paths, beds, ponds and existing trees, then drag guilds into place, or tap one and tap where it should go. Checks warn about overlapping canopies, branches over the boundary and guilds in a building's noon shadow. The 3D view of the whole garden uses this layout, with buildings casting shadows and the sun from true south.
- **Preparing the ground**: five methods with steps, effort, cost and evidence (Charles Dowding's cardboard and compost, Geoff Lawton's sheet mulching with support species, Paul Gautschi's Back to Eden wood chip, a light-proof cover for a season, and one-off digging followed by a sown ground cover), a picker that recommends methods for your plot, a materials calculator and a note on choosing safe cardboard.
- **Soil life**: a hoverable cross-section of the soil food web, how soil builds step by step, current research rated as well supported, emerging, contested or practitioner ideas, and what it means for a guild.
- **Chickens, soil and compost**: UK rules first (registering every flock, the ban on feeding kitchen scraps, bird flu biosecurity), five ways to put hens to work (Geoff Lawton's compost-turning flock, a chicken tractor to prepare ground, the Edible Acres compost run adapted for UK law, deep litter, and hens following other animals or the harvest), the research on chickens and soil rated by strength, and how to fit hens into a forest garden.
- **UK growing notes**: planting season, summer pruning of stone fruit, frost pockets, pollination groups, mulching and planning for shade.

## Editing the plants

All data lives in the `<script>` at the bottom of `index.html`:

- `PLANTS`: companion plants, with layer, jobs, harvest months and yield per plant (young / mature, kg).
- `SPACING`: planting density for herbaceous and ground cover plants (spacing in cm, plants per m², or sowing rate).
- `TREES`: centre trees, with rootstocks, calendars, pruning notes and the suggested guild.

Tree sizes, pruning times and pollination advice follow the RHS guides linked on the page. Yields are estimates from typical nursery figures, not guarantees.

## Hosting

Because it's one static file, GitHub Pages works: Settings → Pages → deploy from the branch root.
