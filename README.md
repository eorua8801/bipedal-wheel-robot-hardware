# Bipedal Wheel Robot — Hardware

Open-source hardware for a self-balancing bipedal wheel robot.
Licensed under the [CERN Open Hardware Licence v2](LICENSE).

---

## Repository Structure

```
/
├── CAD/
│   ├── Assembly/          # Full assembly and sub-assembly CAD files
│   └── Print/             # 3D-printable parts (FDM, PLA, Black)
├── BOM/
│   └── BOM.md             # Bill of Materials
├── README.md
└── README_ko.md
```

---

## 3D Printing

All print parts are designed for FDM printing in black PLA.
The robot is **bilaterally symmetric** — the same files are used for both legs.

| File | Qty per leg | Note |
|------|------------|------|
| BalanceArm_R | 2 | |
| Head_R | 1 | |
| LowerArm_Bearing_R | 1 | |
| LowerArm_Motor_R | 1 | |
| UpperArm_Bearing_R | 1 | |
| UpperArm_Motor_R | 1 | |
| Wheel_R | 1 | |

---

## Assembly Files

| File | Description |
|------|-------------|
| assembled_with_removable_components | Full robot assembly |
| head_cover | Head cover panel |
| Wheel Robot_origin set | Base frame without head cover and battery |

CAD files are available in F3D, STEP, STL, and 3MF formats.

---

## Panels

The wiring board and head cover are cut from **Foamex (PVC foam board), 3t, 300×450mm**.
- Head cover attaches to the frame via 135° corner brackets.
- If a 3D printer is available, printing the head cover is also an option.
- The multi-layer wiring board uses **45mm PCB standoff bolts** as pillars between layers.

---

## Key Components

See [BOM/BOM.md](BOM/BOM.md) for the full bill of materials.

### Required
- **Motor**: Robstride O4 ×4

### Optional (user's choice)
- **LiDAR**: Unitree L2
- **Camera**: General module or Intel RealSense D435

---

## License

CERN Open Hardware Licence Version 2 — see [LICENSE](LICENSE).
