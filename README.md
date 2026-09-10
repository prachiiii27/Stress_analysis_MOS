# Stress Analysis of Circular Shafts — MOS Project 🔩

> **Group 10 | Mechanics of Solids (MOS) Course, IIT Gandhinagar**

A Python-based computational and visualization tool for the **torsional stress analysis** of circular shafts subjected to multiple twisting moments under both **Fixed-Fixed** and **Fixed-Free (Cantilever)** boundary conditions.

---

## 📌 Project Objectives

Automate and visualize the complete torsional response of solid and hollow circular shafts:

1. **Internal Torque Diagram ($T(x)$):** Variation of internal torque along the length of the shaft.
2. **Maximum Shear Stress ($	au_{\text{max}}$):** Elastic torsional shear stress distribution.
3. **Angle of Twist ($\phi(x)$):** Rotation along the shaft axis.
4. **Statically Indeterminate Analysis:** Compatibility equation solver for Fixed-Fixed end conditions.
5. **Cross-Sectional Comparison:** Structural efficiency evaluation of Solid vs. Hollow shafts under identical loads.

---

## 📁 Repository Contents

| File | Description |
| :--- | :--- |
| `MOS_Project_Grp10 (1).ipynb` | Complete Jupyter Notebook containing analytical solvers, SymPy derivations, numerical simulations, and interactive Matplotlib plots |
| `mos-2.pdf` | Final project technical report detailing theory, boundary value problem formulation, and sample case studies |

---

## 🧮 Theoretical Background

### Elastic Torsion Formula
$$\tau = \frac{T \cdot r}{J}$$

Where:
- $T$ = Internal twisting torque ($	ext{N}\cdot\text{m}$)
- $r$ = Radial distance from centroidal axis ($	ext{m}$)
- $J$ = Polar moment of inertia ($	ext{m}^4$)  
  - For solid shaft: $J = \frac{\pi D^4}{32}$  
  - For hollow shaft: $J = \frac{\pi (D_o^4 - D_i^4)}{32}$

### Angle of Twist
$$\phi = \int_0^L \frac{T(x)}{G \cdot J(x)} \, dx = \sum \frac{T_i L_i}{G_i J_i}$$

Where $G$ is the Shear Modulus ($	ext{GPa}$).

### Support Conditions

| Boundary Condition | Statics Classification | Solution Technique |
| :--- | :--- | :--- |
| **Fixed-Free** | Statically Determinate | Direct equilibrium ($\Sigma T_x = 0$) from free end |
| **Fixed-Fixed** | Statically Indeterminate | Equilibrium + Compatibility constraint ($\phi_{\text{total}} = 0$) |

---

## 📊 Generated Visualizations

- Continuous internal torque distribution graphs
- Maximum shear stress envelopes ($	au_{\text{max}}$ vs $x$)
- Angular deformation profiles ($\phi$ vs $x$)
- Comparative stress contours for Solid vs. Hollow sections

---

## 💻 How to Run

1. Clone or download the repository.
2. Launch Jupyter Notebook or Google Colab:
   ```bash
   jupyter notebook "MOS_Project_Grp10 (1).ipynb"
   ```
3. Set your parameters (shaft lengths, diameters, applied torque values, material properties).
4. Run all cells to obtain analytical solutions and high-resolution diagrams.

---

## 👤 Author

**Prachi Jindal**  
Junior Undergraduate, Mechanical Engineering  
Indian Institute of Technology Gandhinagar (IITGN)
