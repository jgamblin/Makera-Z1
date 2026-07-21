# First Coin Laser Test

First laser engraving project using two SVG designs for a double-sided coin concept.

| Field | Value |
|---|---|
| Date started | 2026-07-21 |
| Machine mode | Laser |
| Material | TBD (recommended: painted slate coaster, anodized aluminum card, or basswood) |
| Status | Planning |

## Files In This Folder

| File | Purpose |
|---|---|
| coin-front.svg | Front side artwork |
| coin-back.svg | Back side artwork |

## Goal

Create a clean first-pass engrave of both sides, learn the Z1 laser workflow, and capture settings that can be repeated.

## Step-By-Step Walkthrough

1. Pick a beginner-friendly material.
- Best first try: basswood or masking-taped plywood.
- Avoid reflective metals on run one.

2. Prepare safety and machine.
- Turn on ventilation or fume extraction.
- Wear laser-rated eye protection for 445 to 450 nm if your setup requires it.
- Confirm no flammable clutter near the machine.

3. Open your laser software.
- Use LightBurn or Makera CAM laser workflow.
- Set units to millimeters.

4. Import front art.
- Import coin-front.svg.
- Scale to target size (example: 35 mm diameter).
- Set operation to line or fill depending on artwork style.

5. Import back art in a second file or layer group.
- Import coin-back.svg.
- Match the exact same outer diameter as the front.
- Keep a center mark or alignment reference if you plan to flip the material.

6. Start with conservative test settings.
- Run a small test square first, then the real job.
- Suggested starting points for basswood engraving:
  - Power: 20 to 35%
  - Speed: 1200 to 2400 mm/min
  - Passes: 1
- If engraving is faint, increase power in small steps (5%) before slowing speed.

7. Frame and verify origin.
- Use frame/bounds preview to confirm position.
- Set origin to lower-left or center and stay consistent for both sides.

8. Run the front side.
- Stay at the machine for the first minute.
- Pause immediately if smoke build-up or flare occurs.

9. Flip and align for the back side.
- Use a simple corner jig, tape stops, or registration pins.
- Re-home material against the same references.
- Run coin-back.svg.

10. Inspect and log results.
- Note material, power, speed, passes, and focus height.
- Save final settings in ../../materials-and-settings/materials-log.csv.

## Suggested First-Run Record

| Side | Material | Power (%) | Speed (mm/min) | Passes | Result |
|---|---|---:|---:|---:|---|
| Front | | | | | |
| Back | | | | | |

## Common Fixes

- Too light: increase power slightly or reduce speed.
- Burnt edges: reduce power or increase speed.
- Blurry lines: re-check focus and secure material better.
- Front/back mismatch: improve jig references and keep one consistent origin mode.
- Text not detected in CAM: convert text to paths/outlines in your design app, then re-export SVG.

## If Text Still Does Not Import

Some CAM tools ignore SVG `<text>` elements and only read path geometry.

1. Open the SVG in LightBurn, Inkscape, or Illustrator.
2. Select all text objects.
3. Convert text to paths/outlines.
4. Save as a new file, for example `coin-back-outlined.svg`.
5. Re-import that outlined SVG into your laser workflow.

## Next Improvement Ideas

- Add a dedicated flip jig in this folder with dimensions.
- Save a LightBurn project file with locked alignment layers.
- Create a second pass profile for deeper contrast.
