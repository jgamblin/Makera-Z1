# Resources

Quick-access reference material: cheat sheets, fixture layouts, wiring diagrams, and links to the best community resources for the Makera Z1.

---

## 📐 Feeds & Speeds Cheat Sheet

A condensed pocket reference. Full tested values are in [`/materials-and-settings/`](../materials-and-settings/).

### CNC — 3.175 mm (1/8″) 2-Flute Carbide End Mill

| Material | Feed (mm/min) | Speed (RPM) | DOC (mm) | WOC (mm) |
|---|---|---|---|---|
| Aluminium 6061 | 400–600 | 18 000–22 000 | 0.3–0.5 | 1–1.5 |
| Brass C360 | 300–400 | 16 000–18 000 | 0.2–0.4 | 0.8–1.2 |
| Hardwood | 800–1 500 | 18 000–24 000 | 1–3 | 1.5–3 |
| MDF | 1 000–1 800 | 20 000–24 000 | 2–4 | 2–4 |
| Acrylic (cast) | 600–1 000 | 16 000–20 000 | 0.5–1.5 | 1–2 |

### Laser — 5 W Diode, 450 nm

| Material | Power (%) | Speed (mm/s) | Passes |
|---|---|---|---|
| Anodized aluminium | 70–85 | 80–120 | 1 |
| Plywood 3 mm (cut) | 100 | 8–12 | 3–4 |
| Acrylic 3 mm (engrave) | 35–45 | 350–450 | 1 |
| Leather 2 mm (cut) | 75–85 | 12–18 | 2 |

---

## 🔌 Wiring & Pinout Reference

*(Add wiring diagrams, connector pinouts, and custom harness documentation here.)*

Suggested files to add:
- `z1-controller-pinout.svg` — controller board connector diagram
- `laser-module-wiring.svg` — laser module harness
- `rotary-axis-wiring.svg` — rotary attachment wiring

---

## 📏 Fixturing Diagrams

*(Sketch or photograph your common fixture setups and drop images / DXF files here.)*

Suggested diagrams:
- Vise stop positions for repeated stock loading
- Vacuum plate zone layout
- Hold-down clamp standard positions for 100 × 100 mm stock

---

## 🧲 G-code / Grbl Quick Reference

| Command | Description |
|---|---|
| `G28` | Return to home |
| `G90` | Absolute positioning |
| `G91` | Incremental / relative positioning |
| `G92 X0 Y0 Z0` | Set current position as Work Zero |
| `M3 S___` | Spindle on clockwise at given RPM |
| `M5` | Spindle off |
| `M8` / `M9` | Coolant on / off |
| `F___` | Set feed rate (mm/min) |
| `$H` | Grbl homing cycle |
| `?` | Grbl status query |

---

## 🔗 Community & Official Links

| Resource | URL |
|---|---|
| Makera official site | https://makera.com/ |
| Makera community forum | *(link when available)* |
| LightBurn documentation | https://docs.lightburnsoftware.com/ |
| Fusion 360 CAM tutorials | https://www.autodesk.com/products/fusion-360/blog |
| Grbl project | https://github.com/grbl/grbl |
| CNC Cookbook feeds & speeds | https://www.cnccookbook.com/ |
| r/hobbycnc (Reddit) | https://www.reddit.com/r/hobbycnc/ |
| r/lasercutting (Reddit) | https://www.reddit.com/r/lasercutting/ |

---

## 📚 Recommended Reading / Watching

- *Machinery's Handbook* — authoritative machining reference
- CNC Cookbook's "G-Wizard" feeds & speeds methodology (free articles)
- LightBurn YouTube channel — official tutorials
- NYC CNC YouTube channel — practical Fusion 360 CAM walkthroughs
