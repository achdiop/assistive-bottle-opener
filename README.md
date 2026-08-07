# 💁‍♂️✨ Assistive 3D-Printed Bottle Opener 🖨️🧵

An assistive mechanical device designed to help elderly individuals and people with arthritis or limited grip strength open bottle caps with minimal effort. Built as a course project for **Engineering Workshop**.

![Status](https://img.shields.io/badge/status-functional%20prototype-yellow)
![Tool](https://img.shields.io/badge/CAD-Autodesk%20Fusion-orange)
![Made with](https://img.shields.io/badge/manufacturing-3D%20Printed-blue)

---

## 🗺️ Overview

Opening a bottle cap requires a firm pinch grip and rotational torque — both of which can be painful or impossible for people with arthritis, reduced hand strength, or limited dexterity. This project is a compact, self-centering mechanical gripper that converts a simple rotational input into a strong, evenly-distributed clamping force on the bottle cap, so the user only needs to twist the top disc rather than squeeze and turn a bottle cap directly.

The mechanism works like a **4-jaw self-centering scroll chuck** (similar in principle to a lathe chuck or a camera iris): rotating the top disc drives four bolts through curved slots, which pass through straight radial slots below, converting rotation into simultaneous inward radial motion — closing all four contact points evenly around the cap before the continued rotation actually turns it.

## 🤔 How It Works

1. **Place** the device over a bottle cap.
2. **Rotate the Facecam (top disc) anti-clockwise.**
3. As the Facecam rotates, the four 5 mm bolts — constrained by the Facecam's curved slots above and the Base's straight linear slots below — are driven radially inward.
4. This motion pulls the four gripping jaws inward until they clamp evenly around the bottle cap (self-centering, like a chuck).
5. **Continued rotation** past the clamping point transmits torque through the jaws, unscrewing the cap.

## 🛠️ Assembly & Components

| Part | Description |
|---|---|
| **Facecam (Upper Gear)** | Top-facing disc with a knurled outer rim for thumb grip, four curved (arc) slots for the 5 mm bolts, and a central hole for the 2 mm pivot bolt. |
| **Base** | Middle disc with four straight (linear) radial slots. Constrains the bolts to move radially as the Facecam rotates above it. |
| **Jaws** | Cross/spider-shaped plate beneath the Base. The four 5 mm bolts thread into the ends of its arms; a central hex bore takes the 2 mm alignment bolt. This is the part that physically closes around the bottle cap. |
| **Fasteners** | 4 × 5 mm bolts (drive the cam-slot mechanism and connect Facecam → Base → Jaws) + 1× 2 mm bolt (central pivot/alignment pin for all three plates). |

**Approximate footprint:** ~120 mm diameter × ~63 mm height (fits comfortably in an average adult hand).

## 📂 Repository Contents

```
├── Assembly.stl        # Final assembled model (all parts, bolted position) - stl
├── Assembly.f3z        # Final assembled model (all parts, bolted position) - Fusion Assembly File
├── /CAD                # Autodesk Fusion source files (per-part + assembly)
├── /STL                # Individual part STLs for printing
└── README.md
```

## ⚙️ Technologies Used

- **Autodesk Fusion** — parametric 3D modeling of all components and the assembly
- **3D Printing (FDM)** — physical prototyping of Facecam, Base, and Jaws
- **Engineering Drawings** — early mechanism validation before committing to printed parts
- **Wood Lathe Machine** — cynlindrical wooden jaws.

## ✅ Current Status

The prototype is **fully functional** — the scroll-cam mechanism correctly self-centers and applies rotational torque to a bottle cap. The one outstanding issue is **jaw grip strength**: the current jaw tips are bare printed bolt shafts, which give low-friction, small-area point contact and can slip on smooth or worn caps.

### Planned Improvements
- [ ] Add soft TPU/silicone tips or sleeves to the jaw contact points for higher-friction, compliant grip
- [ ] Increase jaw contact area (e.g. concave pads that wrap around the cap edge)
- [ ] Add serrations/ridges at the jaw tips to bite into cap knurling
- [ ] Explore dual-material printing (rigid body + flexible tip) for a one-print solution

## ▶️ Getting Started (Printing Your Own)

1. Slice `Assembly.stl` (or the individual part files, if using per-part STLs) with your preferred slicer.
2. Print the Facecam, Base, and Jaws in a rigid filament (PLA/PETG recommended).
3. Assemble using 4× M5 bolts and 1× M2 bolt as described above.
4. Hand-tighten only — the mechanism should rotate smoothly without binding.

## 📚 Course Context

This project was developed for the **Engineering Workshop** course as an exercise in mechanism design, parametric CAD modeling, and rapid prototyping via 3D printing.

## 🤝 Team

| Name | Contribution |
| :--- | :--- |
| [**Abbas Dar**](https://github.com/achdiop) | All the CAD models for 3d printing along with assembling the structure. |
| [**Asadullah bin Masood**](https://github.com/oddlyyesterday) | Research for ideation of the inward tightening mechanism the wood lathe machine operation for the jaws. |
| [**Zubia Rani**](https://github.com/ZubiaRani) | Engineering drawings and the wood lathe machine operation for the jaws. |
