# Stress Analysis of Circular Shafts â€” MOS Project

**Group 10 | Mechanics of Solids (MOS) Course, IIT Gandhinagar**

A Python-based computational tool for **torsional stress analysis** of circular shafts under two simultaneous twisting loads, for both **Fixed-Fixed** and **Fixed-Free (Cantilever)** support conditions.

---

## Project Objectives

Automate and visualise the complete torsional analysis of solid and hollow circular shafts:

1. **Internal Torque Diagram** â€” how torque varies along the shaft length under each boundary condition
2. **Maximum Shear Stress** â€” computed from the polar moment of inertia
3. **Angle of Twist** â€” total and cumulative twist along the shaft
4. **Support Reactions** â€” statically indeterminate reactions for Fixed-Fixed configuration
5. **Cross-section Comparison** â€” Solid vs. Hollow shaft under identical loading

---

## Repository Contents

| File | Description |
|------|-------------|
| `MOS_Project_Grp10 (1).ipynb` | Jupyter notebook â€” full analysis, plots, and results |
| `mos-2.pdf` | Project report â€” methodology, equations, and findings |

---

## Theory Covered

### Torsion Formula
```
tau = (T * r) / J
```
Where:
- T = applied torque (N.m)
- r = radial distance from neutral axis (m)
- J = polar moment of inertia (m^4)

### Angle of Twist
```
phi = (T * L) / (G * J)
```
Where G is the shear modulus of the material.

### Support Conditions Analysed

| Condition | Description |
|-----------|------------|
| Fixed-Free | One end fixed, other end free â€” statically determinate |
| Fixed-Fixed | Both ends fixed â€” statically indeterminate; reactions solved via compatibility equation |

---

## Outputs

- Torque distribution diagram along shaft length
- Shear stress profile
- Angle of twist plot
- Comparison between solid and hollow cross-sections
- Tabulated results for each shaft segment

---

## Tools and Libraries

```python
import numpy as np
import matplotlib.pyplot as plt
import sympy  # for symbolic solution of indeterminate reactions
```

---

## How to Run

1. Open `MOS_Project_Grp10 (1).ipynb` in Jupyter Notebook or Google Colab.
2. Set shaft geometry, material properties, load positions, and support type.
3. Run all cells to generate torque, stress, and twist diagrams.

---

## Author

**Prachi Jindal** â€” Junior Undergraduate, Mechanical Engineering, IIT Gandhinagar