# Tool Library

Exported tool definitions for the software packages used with the Makera Z1. Import these files directly into your CAM software so feeds, speeds, and geometry are pre-loaded.

---

## Folder Structure

```
tool-library/
├── makera-cam/        # Tool tables for Makera CAM
├── lightburn/         # Material library / cut settings presets (.clb)
├── fusion-360/        # Fusion 360 tool library (.json)
└── vcarve/            # VCarve / Aspire tool database (.vtdb)
```

---

## How to Import

### Makera CAM
*(Describe import steps once you have exported a library from Makera CAM.)*

### LightBurn
1. Open LightBurn → **Edit → Material Library**.
2. Click **Import** and select the `.clb` file from `lightburn/`.

### Fusion 360
1. Open Fusion 360 → **Manufacture** workspace.
2. In the **Tool Library** panel, click **Import** and select the `.json` file from `fusion-360/`.

### VCarve / Aspire
1. Open VCarve → **Toolpaths → Tool Database**.
2. Click **Import Tools** and select the `.vtdb` file from `vcarve/`.

---

## Bit / End Mill Inventory

Keep this table updated as tools are purchased, worn, or retired.

| Tool | Diameter | Flutes | Material | # on Hand | Condition | Notes |
|---|---|---|---|---|---|---|
| Flat end mill | 3.175 mm (1/8″) | 2 | Carbide | 4 | Good | General-purpose |
| V-bit | 60° | — | Carbide | 2 | Good | Engraving, PCBs |
| Ball nose | 3.175 mm | 2 | Carbide | 2 | Good | 3D surfacing |
| Drill | 1.0 mm | — | Carbide | 5 | Good | PCB drilling |
| Drag knife | — | — | — | 1 | Good | Vinyl / paper |

---

## Adding a New Tool

1. Create or export the tool definition from your CAM software.
2. Place the file in the appropriate subfolder above.
3. Add a row to the inventory table.
4. Commit with a message like `tool-library: add 1/8" 2-flute Fusion 360 definition`.
