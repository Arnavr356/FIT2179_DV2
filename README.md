Australia's Threatened Species Crisis
FIT2179 Data Visualisation 2 — Monash University, Semester 1 2026
A data visualisation exploring Australia's biodiversity emergency, built with Vega-Lite, HTML and CSS.
Live Visualisation
View at: https://[your-github-username].github.io/FIT2179_DV2/
Structure
FIT2179_DV2/
├── index.html          # Main visualisation page
├── style.css           # Nature-themed design system
├── data/               # All data sources (JSON + CSV)
│   ├── species_clean.csv          # 2,098 EPBC-listed threatened species
│   ├── communities_clean.csv      # 111 threatened ecological communities
│   ├── group_status.json          # Species counts by group × threat status
│   ├── group_totals.json          # Group totals (CE/EN/VU)
│   ├── crit_ratio.json            # % critically endangered per group
│   ├── status_totals.json         # Species vs communities by status
│   ├── state_species.json         # Threatened species per state × status
│   ├── state_communities.json     # Threatened communities per state × status
│   ├── communities_by_state.json  # Community totals per state (lollipop data)
│   ├── state_total.json           # Per-state summary totals
│   ├── vertebrate_detail.json     # Five vertebrate groups × status with %
│   ├── top_communities.json       # Most widespread threatened communities
│   ├── comm_status.json           # Community status breakdown (111 total)
│   ├── heatmap_animals.json       # Animal group × state counts (from CSV)
│   ├── map_labels.json            # State label coordinates for map
│   └── australia-states.json     # GeoJSON boundaries for all 8 jurisdictions
└── specs/              # Individual Vega-Lite JSON specs (human-readable)
    ├── chart-group-stacked.json
    ├── chart-crit-ratio.json
    ├── chart-dot-strip.json
    ├── chart-status-compare.json
    ├── chart-map.json
    ├── chart-state-species.json
    ├── chart-communities-lollipop.json
    ├── chart-heatmap.json
    ├── chart-top-communities.json
    ├── chart-comm-status.json
    ├── chart-scatter.json
    ├── chart-vertebrate-norm.json
    └── chart-waffle-note.md
Data Sources

Department of Climate Change, Energy, the Environment and Water
— Threatened Species State Lists via data.gov.au
Atlas of Living Australia
— Species occurrence data (state-level counts) via ALA

Visualisation Charts
#ChartIdiom1Threatened species by biological groupStacked bar2Critically endangered ratio per groupHorizontal bar + reference line3Species count by groupDot strip (circle + rule)4Species vs communities by statusGrouped bar5Total threatened listings per stateChoropleth map6Species by state and threat levelInteractive stacked bar (click to filter)7Communities per stateLollipop chart8Animal group × stateHeatmap (rect)9Most widespread threatened communitiesHorizontal bar10Community status breakdownDonut/arc11Species vs communities per stateBubble scatter12Vertebrate threat compositionNormalised 100% stacked bar13CE share for Fish/Frogs/ReptilesFaceted waffle charts
Author
Arnav Raj — Student ID 34484515
FIT2179 Data Visualisation, Monash University
June 2026