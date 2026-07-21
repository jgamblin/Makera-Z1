# Maintenance Log

This folder tracks everything needed to keep the Makera Z1 running reliably: calibration history, firmware updates, spindle hours, lubrication schedule, and hardware modifications.

---

## 📅 Calibration History

| Date | Axis / Parameter | Before | After | Method | Notes |
|---|---|---|---|---|---|
| 2026-01-01 | XY squareness | — | 0.05 mm / 200 mm | Dial indicator + reference square | Initial setup |
| 2026-01-01 | Z-probe offset | — | calibrated | Makera CAM auto-probe | Initial setup |

---

## 💾 Firmware & Software Versions

| Date | Component | Previous Version | New Version | Notes |
|---|---|---|---|---|
| 2026-01-01 | Makera Z1 firmware | — | v1.0.0 | Initial flash |
| 2026-01-01 | Makera CAM | — | v1.0.0 | Initial install |
| 2026-01-01 | LightBurn | — | v1.7.x | Initial install |

---

## ⏱ Spindle Hours Log

Track cumulative spindle hours to know when to inspect bearings and brushes.

| Date | Session Hours | Cumulative Total | Notes |
|---|---|---|---|
| 2026-01-01 | 0.5 | 0.5 | Initial calibration run |

---

## 🛢 Lubrication Schedule

| Interval | Component | Lubricant | Last Done | Next Due |
|---|---|---|---|---|
| Every 20 h | Z-axis lead screw | PTFE dry lube | 2026-01-01 | *(calculate)* |
| Every 20 h | X/Y linear rails | Light machine oil | 2026-01-01 | *(calculate)* |
| Every 50 h | All axes | Full inspection + re-lube | — | — |

---

## 🔩 Hardware Modifications

Document any physical modifications to the machine here.

| Date | Modification | Reason | Files / Links | Notes |
|---|---|---|---|---|
| | | | | |

---

## 🐛 Issues & Fixes

| Date | Symptom | Root Cause | Fix Applied | Status |
|---|---|---|---|---|
| | | | | |

---

## 📝 Notes

- Always home the machine before and after a maintenance session.
- Keep a copy of the factory firmware file before applying any updates.
- After lubrication, run all axes through full travel 5× before cutting.
