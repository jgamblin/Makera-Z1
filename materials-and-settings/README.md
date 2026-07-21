# Materials & Settings

A central reference database for every material tested on the Makera Z1. The tables below are quick references; the full logged history lives in [`materials-log.csv`](./materials-log.csv).

> **Note:** All settings are starting points. Your results will vary based on tool sharpness, material batch, fixturing rigidity, and ambient temperature. Always run a test cut before a production job.

---

## ⚡ Laser Quick-Reference (5 W Diode, 450 nm)

### Engraving

| Material | Power (%) | Speed (mm/s) | Passes | Air Assist | Notes |
|---|---|---|---|---|---|
| Anodized aluminium (black) | 80 | 100 | 1 | Off | Removes anodizing cleanly |
| Anodized aluminium (coloured) | 70 | 120 | 1 | Off | Lighter colour = lower power |
| Bare brass | 100 | 50 | 3 | On | Use Cermark/Dry-moly for marking |
| Plywood (3 mm) | 60 | 300 | 1 | On | Grain direction affects depth |
| MDF (3 mm) | 55 | 250 | 1 | On | Very dusty — strong extraction |
| Acrylic (cast, 3 mm) | 40 | 400 | 1 | Off | Frosted finish |
| Acrylic (extruded, 3 mm) | 35 | 350 | 1 | Off | Extruded engraves less crisply |
| Leather | 50 | 200 | 1 | On | Test scrap first — varies widely |
| Cardstock / paper | 20 | 500 | 1 | Off | |

### Cutting

| Material | Power (%) | Speed (mm/s) | Passes | Air Assist | Notes |
|---|---|---|---|---|---|
| Plywood (3 mm) | 100 | 10 | 3 | On | Elevate off bed for clean back |
| MDF (3 mm) | 100 | 8 | 4 | On | |
| Acrylic (cast, 3 mm) | 100 | 6 | 4 | Off | Air assist can cause flaming |
| Cardstock | 60 | 50 | 1 | Off | |
| Leather (2 mm) | 80 | 15 | 2 | On | |

---

## 🔧 CNC Mill Quick-Reference

### Anodized / Bare Aluminium (6061)

| Operation | Tool | Feed (mm/min) | Plunge (mm/min) | Speed (RPM) | WOC | DOC | Notes |
|---|---|---|---|---|---|---|---|
| Adaptive rough | 3.175 mm 2-fl | 500 | 150 | 20 000 | 1.5 mm | 0.5 mm | Flood/mist recommended |
| Contour finish | 3.175 mm 2-fl | 400 | 150 | 22 000 | 0.2 mm | 5 mm | |
| Engrave / V-carve | 60° V-bit | 300 | 100 | 18 000 | — | 0.3 mm | |

### Brass (C360 Free-Machining)

| Operation | Tool | Feed (mm/min) | Plunge (mm/min) | Speed (RPM) | WOC | DOC | Notes |
|---|---|---|---|---|---|---|---|
| Adaptive rough | 3.175 mm 2-fl | 350 | 100 | 16 000 | 1 mm | 0.3 mm | Lubricate with cutting oil |
| Contour finish | 3.175 mm 2-fl | 300 | 100 | 18 000 | 0.1 mm | 3 mm | |

### Hardwood (Oak, Maple)

| Operation | Tool | Feed (mm/min) | Plunge (mm/min) | Speed (RPM) | WOC | DOC | Notes |
|---|---|---|---|---|---|---|---|
| Pocket / 2D contour | 3.175 mm 2-fl | 1 200 | 400 | 22 000 | 2 mm | 1.5 mm | Climb milling preferred |
| V-carve | 60° V-bit | 800 | 300 | 20 000 | — | variable | |
| Profile cut | 3.175 mm 2-fl | 1 000 | 400 | 22 000 | full | 3 mm | Tabs recommended |

### Acrylic (Cast)

| Operation | Tool | Feed (mm/min) | Plunge (mm/min) | Speed (RPM) | WOC | DOC | Notes |
|---|---|---|---|---|---|---|---|
| Pocket | 3.175 mm 2-fl | 1 000 | 300 | 18 000 | 2 mm | 1 mm | Chip clearing critical |
| Profile cut | 3.175 mm 2-fl | 800 | 250 | 16 000 | full | 2 mm | Multi-pass; freeze bit if melting |

---

## 📋 Full Materials Log

See [`materials-log.csv`](./materials-log.csv) for a row-by-row record of every tested setting including date, notes, and pass/fail result.
