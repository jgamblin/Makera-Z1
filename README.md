# Makera Z1 — Open Lab

> **A public learning lab documenting the capabilities, projects, and workflow of the [Makera Z1](https://makera.com/) — a hybrid desktop CNC mill and 5 W diode laser engraver.**

This repository is a living record of everything I machine and engrave: vector art, 3D models, G-code programs, custom CAM tool libraries, material test results, and full project write-ups. Nothing here is polished marketing material — it's real-world notes, failures, and fixes.

---

## 📂 Repository Navigation

| Folder | Contents |
|---|---|
| [`/projects/`](./projects/) | Individual build folders, each self-contained with source files, G-code, and a project README |
| [`/materials-and-settings/`](./materials-and-settings/) | Quick-reference parameter tables + a structured CSV log for every material tested |
| [`/tool-library/`](./tool-library/) | Exported tool definitions for Makera CAM, LightBurn, Fusion 360, and VCarve |
| [`/maintenance/`](./maintenance/) | Calibration dates, firmware changelogs, spindle hours, lubrication schedule, and hardware mods |
| [`/resources/`](./resources/) | Cheat sheets, fixture diagrams, wiring references, and curated community links |

---

## 🛠 Hardware & Setup

### Machine Specs

| Attribute | Value |
|---|---|
| Machine | Makera Z1 |
| Work area (XY) | 200 × 200 mm (nominal) |
| Z travel | ~50 mm |
| Spindle | Brushless 10 000–24 000 RPM |
| Laser module | 5 W diode (450 nm blue) |
| Controller | Makera proprietary / grbl-based |
| Software | Makera CAM, LightBurn (laser), Fusion 360, VCarve |
| Connectivity | USB / Wi-Fi |

### Bits & End Mills on Hand

| Tool | Diameter | Flutes | Material Suitability |
|---|---|---|---|
| Flat end mill | 3.175 mm (1/8″) | 2 | Wood, acrylic, soft metals |
| V-bit | 60° | — | Engraving, PCB isolation |
| Ball nose | 3.175 mm | 2 | 3D surfacing, wood |
| Drill bit | 1.0 mm | — | PCB drilling |
| Drag knife | — | — | Vinyl, paper |

### Optional Accessories

- Rotary axis attachment
- Vacuum workholding plate
- Enclosure / fume extractor
- Probe / tool-length sensor
- Laser safety enclosure panel

---

## ✅ Safety & Pre-Flight Checklist

Run through this list **before every job**.

| # | Check | ✓ |
|---|---|---|
| 1 | Ventilation on / fume extractor running | ☐ |
| 2 | Laser safety glasses worn (OD4+ 445–450 nm) | ☐ |
| 3 | Enclosure door closed (laser jobs) | ☐ |
| 4 | Workpiece securely clamped / vacuum engaged | ☐ |
| 5 | Tool correctly seated and collet torqued | ☐ |
| 6 | Z-probe run; Work Coordinate System (WCS) zeroed | ☐ |
| 7 | XY datum / corner confirmed in CAM preview | ☐ |
| 8 | Spindle / laser speed matches CAM program | ☐ |
| 9 | Feed-hold and E-stop accessible | ☐ |
| 10 | No loose clothing, hair, or cables near spindle | ☐ |
| 11 | Fire extinguisher within arm's reach | ☐ |
| 12 | First 30 s: observe machine closely, finger on feed-hold | ☐ |

---

## 📐 Quick-Start Workflow

```
Design (Fusion 360 / Inkscape / LightBurn)
  │
  ▼
CAM / laser path setup (Makera CAM / LightBurn / VCarve)
  │
  ▼
Pre-flight checklist ✓
  │
  ▼
Send to machine → observe → adjust
  │
  ▼
Log results in /materials-and-settings/materials-log.csv
```

---

## 📄 License

Files in this repository are released under the [MIT License](./LICENSE) unless otherwise noted in a project subfolder.

---

*Questions, suggestions, or want to share a parameter that works well? Open an issue or start a discussion.*
