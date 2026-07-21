# Bigfoot 19G Relief

3D relief carve of a Bigfoot design using an STL file.

| Field | Value |
|---|---|
| Date started | 2026-07-21 |
| Machine mode | CNC Mill |
| Material | TBD (recommended: hardwood like Walnut or Maple, or MDF) |
| Estimated machine time | TBD |
| Status | Planning |

## Files In This Folder

| File | Purpose |
|---|---|
| `BIGFOOT19GA.stl` | Main 3D relief model for CAM |
| `BIGFOOT19G.png` | Reference image |
| `BIGFOOT19GA.png` | Reference image / Alpha map |
| `BIGFOOT19G-preview.png` | Screenshot of the model preview |

## Goal

Successfully import an STL into CAM (Fusion 360, VCarve, or Makera CAM) and generate a two-stage 3D toolpath (Roughing and Finishing) to carve a high-detail wood relief.

## Workflow Overview

1. **CAM Setup**
   - Import the STL file.
   - Define the stock size (slightly larger and thicker than the model).
   - Set the origin (usually top-center for 3D reliefs).

2. **Roughing Pass (3D Adaptive / Z-Level Roughing)**
   - **Tool**: 1/4" or 1/8" Flat End Mill.
   - **Purpose**: Clear away the bulk of the material fast.
   - **Leave Stock**: Leave about 0.5 mm to 1.0 mm of stock for the finishing pass.

3. **Finishing Pass (Parallel / 3D Finishing)**
   - **Tool**: 1/8" or 1/16" Tapered Ball Nose End Mill (the finer the tip, the more detail, but the longer the time).
   - **Purpose**: Mill the final high-resolution details.
   - **Stepover**: Keep stepover small (approx 8-12% of the tool's diameter) for a smooth finish requiring less sanding.

4. **Cutout Pass (2D Contour)** *Optional*
   - Cut the finished badge/frame out of the remaining stock.

## Suggested First-Run Record

| Operation | Tool | Feed (mm/min) | Plunge (mm/min) | RPM | Stepdown | Stepover |
|---|---|---:|---:|---:|---:|---:|
| 3D Roughing | Flat End Mill | | | | | |
| 3D Finishing| Ball Nose | | | | | |
