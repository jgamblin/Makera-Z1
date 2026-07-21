# Makera Z1 Open Lab

A public build log and reference library for work done on the [Makera Z1](https://makera.com/) hybrid desktop CNC mill and 5W diode laser.

This repository tracks real machine work: projects, CAM settings, material tests, tooling, and maintenance notes. It is intended as a practical operating notebook, including mistakes, adjustments, and repeatable settings.

## What You Will Find Here

- Project folders with source files, exports, and job notes
- Material test data with settings that worked (and did not)
- Tool library definitions for common CAM workflows
- Maintenance and calibration records
- Quick-reference resources for setup and troubleshooting

## Repository Layout

| Path | Purpose |
|---|---|
| [projects/](./projects/) | Self-contained project folders with assets, outputs, and documentation |
| [materials-and-settings/](./materials-and-settings/) | Material test logs, parameter notes, and [materials-log.csv](./materials-and-settings/materials-log.csv) |
| [tool-library/](./tool-library/) | Reusable tool definitions and presets for CAM and engraving software |
| [maintenance/](./maintenance/) | Calibration notes, firmware history, machine upkeep logs, and modifications |
| [resources/](./resources/) | Cheat sheets, fixtures, wiring references, and external links |

## Quick Start

1. Open [projects/README.md](./projects/README.md) to choose a project structure.
2. Review [materials-and-settings/README.md](./materials-and-settings/README.md) for known-safe starting parameters.
3. Confirm your tooling against [tool-library/README.md](./tool-library/README.md).
4. Run the pre-flight checklist below before cutting or engraving.
5. Log your results in [materials-log.csv](./materials-and-settings/materials-log.csv).

## Machine Snapshot

| Attribute | Value |
|---|---|
| Machine | Makera Z1 |
| Work area (XY) | 200 x 200 mm (nominal) |
| Z travel | About 50 mm |
| Spindle | Brushless, 10,000 to 24,000 RPM |
| Laser module | 5W diode, 450 nm |
| Controller | Makera proprietary, GRBL-based |
| Software | Makera CAM, LightBurn, Fusion 360, VCarve |
| Connectivity | USB, Wi-Fi |

## Pre-Flight Safety Checklist

Use this checklist before every job.

| # | Check | Done |
|---|---|---|
| 1 | Ventilation and fume extraction are running | ☐ |
| 2 | Proper laser safety eyewear is worn for laser jobs | ☐ |
| 3 | Workpiece is securely clamped or vacuum-held | ☐ |
| 4 | Tool is correctly seated and collet is tightened | ☐ |
| 5 | Work zero and Z zero are set and verified | ☐ |
| 6 | CAM preview and machine origin match | ☐ |
| 7 | Feed-hold and emergency stop are immediately accessible | ☐ |
| 8 | First 30 seconds are monitored at the machine | ☐ |

## Standard Workflow

1. Design in CAD or vector tools.
2. Generate toolpaths in CAM.
3. Verify setup and run pre-flight checks.
4. Start job, monitor, and adjust as needed.
5. Record final settings and outcomes for future runs.

## Contributing Notes

Small, practical updates are welcome, especially:

- Material settings validated on real jobs
- Tooling changes with measurable outcomes
- Setup or maintenance notes that improve repeatability

## License

This repository is licensed under the [Apache License 2.0](./LICENSE), unless a subfolder explicitly states otherwise.
