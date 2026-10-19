# Team 3 data package - Tempe

Your mission: Tempe Streetcar carries roughly 790,000 riders a year
(FY2024). Build the mode-choice model that explains who they are.

## What is in this folder
| File | What it is | Used in step |
|---|---|---|
| tempe_links.geojson | Tempe street network with lanes/speed/capacity | 1, 4 - auto background |
| tempe_zones.geojson | Tempe analysis zones | 2 - P/A table |
| tempe_superzones.geojson | The superzone roll-up used in class | aggregation checks |
| tempe_transit_stops.geojson | Transit stops incl. the 14 streetcar stops | 3 - mode availability |
| tempe_transit_shapes_synthesized.geojson | Transit route shapes (synthesized from stops - label them as such) | maps |
| tempe_zones_map.png | Ready-made zone map | model card figure |

## Also yours (already on Canvas / course page)
- `Tempe_Model_Workbench.html` - the interactive Tempe workbench; your
  Master Inventory counts come from it.
- L02/L07 logit workbooks (mode choice), L03 (logsums per mode).

## The reality check (step 5)
Your model's annual streetcar ridership should land within 2x of 790,000.
Annualize a weekday as ~300 equivalent days and say so in the model card.
