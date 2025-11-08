# Bézier-Curve-Based Trajectory Design (Simplified Demonstration)

This repository contains a simplified implementation of the Bézier-curve-based well trajectory design method used as one component of the study  
**“Intelligent Drilling Trajectory Optimization Method Based on Azimuth LWD Data.”**

The code in this repository focuses **only** on the geometric construction of Bézier trajectories under the condition that a reservoir centerline (sweet-spot line) is already known.  
It is intended as a **minimal, non-sensitive demonstration**, and **does not include** any real drilling data or field cases.

Only three basic elements are demonstrated here:

1. A reservoir distribution background image  
2. A reservoir centerline (given as coordinates)  
3. A conventional cubic Bézier trajectory designed to follow the sweet-spot while satisfying curvature constraints

This repository **does not** include sensitive field data, real production wells, LWD measurements, or actual drilling-case trajectory information.

---

## 📂 Repository Contents

### `bezier_trajectory.py`
A self-contained Python script demonstrating:

- Spline fitting of a reservoir sweet-spot line  
- Construction of a cubic Bézier curve segment  
- Adaptive adjustment of control-point spacing  
- Curvature computation for constraint checking  
- Conversion between reservoir coordinates and image pixels  
- Plotting the Bézier trajectory on a reservoir background
- Exporting:
  - Designed trajectory (`设计轨迹_output.xlsx`)
  - Segment parameters (`设计参数_output.xlsx`)

This script illustrates the **geometric principle** of Bézier trajectory formation, not the full closed-loop intelligent control framework used in the complete research.

---

### `reservoir_image.png`
A simplified reservoir background image.  
This image is **synthetic** and provided solely for demonstrating visualization.

### `reservoir_data.csv`
A grid-formatted synthetic reservoir distribution map used for coordinate mapping and plot scaling.

### `path_center_sweet.csv`
A synthetic reservoir centerline (sweet-spot path).  
The trajectory algorithm attempts to follow this line under curvature constraints.

---

## ✅ What This Demonstration Represents

This repository is designed to show:

- How a reservoir sweet-spot line can guide geometric trajectory planning  
- How Bézier curves can construct smooth and curvature-continuous well paths  
- How curvature constraints can be evaluated numerically  
- How designed trajectories overlay on reservoir sections

However, this demonstration **does NOT** include:

✘ Real LWD data  
✘ Real drilling data  
✘ Real field trajectories  
✘ Sensitive engineering parameters  
✘ Any proprietary algorithms or datasets

It is purely a **safe, simplified, reproducible example** illustrating the geometric foundation used in the full study.

---


