<div align="center">

# MetaOrigami

### Origami-Inspired Meta-Structures, Parametric CAD and Digital Fabrication

**Miura-ori · Kresling · Geometric Programmability · CAD · Digital Fabrication**

<p align="center">
  <img src="EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg" width="85%">
</p>

**Undergraduate research project developed by Ana Beatriz Alencar Dias,  
under the supervision of Americo Barbosa da Cunha Junior.**

</div>

---

### Table of Contents

- [Overview](#overview)
- [Miura-ori](#miura-ori)
- [Kresling](#kresling)
- [Miura Alphabet](#miura-alphabet)
- [CAD and Research Files](#cad-and-research-files)
- [Digital Fabrication](#digital-fabrication)
- [Research Scope](#research-scope)
- [Repository Structure](#repository-structure)
- [Authors](#authors)
- [Institutional Support](#institutional-support)
- [Contact](#contact)

---

## Overview

**MetaOrigami** investigates the use of origami geometry as a basis for the
design of reconfigurable structures and origami-inspired metamaterials.

The project combines geometric analysis, parametric CAD modeling and digital
fabrication to study how simple folding cells can generate larger and more
complex spatial structures.

The current research focuses primarily on two origami architectures:

- **Miura-ori**, used as the main platform for parametric modeling,
  tessellation studies and geometric exploration;
- **Kresling**, investigated as a complementary cylindrical origami
  architecture with coupled geometric parameters.

The project also explores **geometric programmability**, in which local
origami-inspired modules are organized to generate prescribed global shapes.

---

## Miura-ori

The **Miura-ori** is a periodic origami pattern based on a tessellation of
parallelogram-shaped facets connected by alternating mountain and valley
creases.

Its geometry allows coordinated folding of the complete tessellation and
provides a useful model for studying compact deployment, geometric coupling and
reconfigurable structures.

Within MetaOrigami, the Miura-ori was used to investigate:

- geometric parameters of the unit cell;
- different folding configurations;
- tessellation size and organization;
- limits associated with face interference;
- parametric CAD modeling;
- generation of larger structures from repeated cells.

### Geometric study

<p align="center">
  <img src="EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg" width="82%">
</p>

The figure above is part of the original project material and illustrates
different Miura-ori configurations explored during the geometric study.

### Miura-ori 7 × 4 model

A complete **7 × 4 Miura-ori structure** was developed in Autodesk Fusion 360.

The model is available in editable CAD and mesh formats.

| File | Format | Description |
|---|---|---|
| [`MiuriOri_7x4.f3d`](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.f3d) | Fusion 360 | Editable CAD model |
| [`MiuriOri_7x4_3D_v6.stl`](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4_3D_v6.stl) | STL | Triangulated 3D geometry |
| [`MiuriOri_7x4.obj`](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.obj) | OBJ | General-purpose 3D model |

---

## Miura-ori Crease Pattern

The planar crease pattern associated with the 7 × 4 model is also included in
the repository.

| File | Format |
|---|---|
| [`MiuraOri_7x4.dxf`](FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.dxf) | DXF |
| [`MiuraOri_7x4.pdf`](FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.pdf) | PDF |

The DXF representation can be used as a basis for CAD inspection and digital
fabrication workflows.

---

## Kresling

The **Kresling pattern** is a triangulated cylindrical origami architecture.

Its folding motion combines axial displacement and rotation, producing a
compact deployable structure whose geometry depends on coupled dimensions and
angles.

In this project, Kresling was investigated as a second origami family after
the Miura-ori study.

The work revealed an important modeling challenge: modifying one geometric
parameter can affect several other quantities required for cylindrical closure.

For this reason, the current Kresling work is considered an **exploratory
geometric investigation** rather than a complete parametric generator.

Current working/reference files include:

```text
Kresling_6gon_A_and_B_TwoInchEdgeLength.dxf
KreslingArrayCreasePattern.dxf
KreslingArrayCreasePattern1.dxf
KreslingArrayCreasePattern1.studio3
```

These files are retained as research material while their provenance and
redistribution conditions are reviewed.
