<div align="center">

# MetaOrigami

### Origami-Inspired Metamaterials, Parametric CAD and Digital Fabrication

**Miura-ori · Kresling · Geometric Programmability · Reconfigurable Structures**

<p align="center">
  <img src="EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg" width="82%" alt="MetaOrigami — Miura-ori geometric study">
</p>

**Undergraduate research project by Ana Beatriz Alencar Dias  
under the supervision of Americo Barbosa da Cunha Junior**

</div>

---

## Table of Contents

- [Overview](#overview)
- [Research Approach](#research-approach)
- [Miura-ori](#miura-ori)
- [Miura-ori CAD Model](#miura-ori-cad-model)
- [Miura-ori Crease Pattern](#miura-ori-crease-pattern)
- [Kresling](#kresling)
- [Miura Alphabet](#miura-alphabet)
- [Available Files](#available-files)
- [Digital Fabrication](#digital-fabrication)
- [Repository Structure](#repository-structure)
- [Authors](#authors)
- [Institutional Context](#institutional-context)
- [Citation](#citation)
- [Contact](#contact)

---

## Overview

**MetaOrigami** is an undergraduate research project focused on the geometric
design and digital prototyping of origami-inspired meta-structures.

The project investigates how a relatively simple local folding pattern can be
repeated, parametrized and reorganized to produce larger structures with
complex global geometries.

The work combines:

- origami geometry;
- parametric CAD modeling;
- crease-pattern design;
- tessellation;
- geometric analysis;
- digital fabrication;
- modular design;
- reconfigurable structures;
- origami-inspired metamaterials.

The main architecture investigated is the **Miura-ori** pattern.  
The **Kresling** pattern is studied as a complementary cylindrical origami
geometry with a more strongly coupled parametrization.

---

## Research Approach

The basic workflow adopted in the project is:

```text
Origami pattern
      ↓
Geometric unit cell
      ↓
Parametric description
      ↓
Crease pattern
      ↓
CAD model
      ↓
Tessellated structure
      ↓
Digital prototype
      ↓
Complex global geometry
```

The central idea is that the geometry of the local cell controls the geometry
and possible transformations of the larger structure.

This relationship between **local rules** and **global form** is one of the
main motivations for studying origami architectures as mechanical
meta-structures.

---

# Miura-ori

## Geometry

The **Miura-ori** is a periodic origami pattern constructed from a tessellation
of parallelogram-like facets connected through alternating mountain and valley
creases.

A single Miura cell can be described using geometric quantities such as:

- facet dimensions;
- acute angle of the parallelogram;
- fold angle;
- orientation of adjacent facets.

When cells are repeated, the complete sheet forms a coordinated mechanism in
which many facets move simultaneously.

The pattern is particularly interesting because changes at the unit-cell level
produce organized transformations of the entire tessellation.

---

## Geometric Study

<p align="center">
  <img src="EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg" width="88%" alt="Miura-ori cells and angular configurations">
</p>

The project investigated different Miura-ori configurations by modifying the
folding geometry and observing the resulting spatial arrangement.

The geometric study was used to analyze:

- different opening configurations;
- relationships between neighboring facets;
- compact and expanded states;
- geometric interference between panels;
- inversion of the expected configuration at large folding angles;
- organization of repeated cells.

The source material for this study is available in PDF, JPG and Adobe
Illustrator formats.

| File | Format |
|---|---|
| [Miuri-Ori_plan_angulos diferentes.pdf](EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.pdf) | PDF |
| [Miuri-Ori_plan_angulos diferentes.jpg](EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg) | JPG |
| [Miuri-Ori_plan_angulos_diferentes.ai](EstudoCelulas/Miuri-Ori_plan_angulos_diferentes.ai) | Adobe Illustrator |

---

# Miura-ori CAD Model

A **7 × 4 Miura-ori tessellation** was developed in Autodesk Fusion 360.

The CAD model provides a computational representation of the folded geometry
and allows the structure to be inspected and reused in different digital
workflows.

The model is available in three formats.

| File | Format | Description |
|---|---|---|
| [MiuriOri_7x4.f3d](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.f3d) | F3D | Autodesk Fusion 360 CAD model |
| [MiuriOri_7x4_3D_v6.stl](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4_3D_v6.stl) | STL | Triangulated 3D geometry |
| [MiuriOri_7x4.obj](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.obj) | OBJ | General-purpose 3D geometry |

### Download

**Fusion 360**

[Download `MiuriOri_7x4.f3d`](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.f3d)

**STL**

[Download `MiuriOri_7x4_3D_v6.stl`](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4_3D_v6.stl)

**OBJ**

[Download `MiuriOri_7x4.obj`](FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.obj)

---

# Miura-ori Crease Pattern

The planar crease pattern associated with the Miura-ori 7 × 4 model is
available as both a vector CAD file and a PDF document.

The crease pattern represents the planar geometric information from which the
folded architecture is constructed.

| File | Format | Description |
|---|---|---|
| [MiuraOri_7x4.dxf](FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.dxf) | DXF | Vector crease geometry |
| [MiuraOri_7x4.pdf](FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.pdf) | PDF | Crease-pattern document |

### Download

[Download the DXF crease pattern](FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.dxf)

[Download the PDF crease pattern](FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.pdf)

---

# Kresling

The **Kresling pattern** is a cylindrical origami architecture composed
primarily of triangular facets arranged around a polygonal cross section.

Its deformation combines two characteristic motions:

**axial displacement** and **rotation**.

As the structure contracts or expands, neighboring rings rotate relative to
one another.

This coupling makes Kresling geometries particularly interesting for the study
of:

- deployable cylinders;
- compact structures;
- torsional mechanisms;
- bistable and multistable architectures;
- geometrically programmable structures.

---

## Kresling Geometric Challenge

Kresling was investigated as a second origami architecture during the project.

Its CAD parametrization proved more demanding than the corresponding Miura-ori
model.

For a closed cylindrical structure, parameters such as:

- number of polygon sides;
- polygon radius;
- cylinder height;
- diagonal dimensions;
- triangular facet angles;
- relative rotation between rings;

cannot generally be modified independently.

Changing one parameter affects other quantities required to preserve geometric
closure.

The current work therefore represents an **exploratory investigation of the
Kresling geometry and its crease patterns**.

---

## Kresling Files

The current repository contains the following Kresling working files:

```text
Kresling_6gon_A_and_B_TwoInchEdgeLength.dxf
KreslingArrayCreasePattern.dxf
KreslingArrayCreasePattern1.dxf
KreslingArrayCreasePattern1.studio3
```

These files document the geometric exploration carried out during this stage
of the research.

---

# Miura Alphabet

One of the main geometric experiments developed from the Miura-ori study was
the construction of a **complete alphabet using Miura-inspired modular
geometries**.

Instead of repeating the same tessellation indefinitely, local modules were
reorganized to generate different recognizable global shapes.

The alphabet provides a visual demonstration of the principle:

```text
local geometric unit
        ↓
controlled organization
        ↓
complex global geometry
```

The experiment demonstrates how a common geometric vocabulary can be used to
construct many distinct macroscopic configurations.

This idea is relevant beyond typography. It provides a simple visual example
of **geometric programmability**, in which the organization of local structural
units determines the form of a larger meta-structure.

The CAD source developed during the project is:

```text
Miura-Ori-Alphabet.f3d
```

---

# Available Files

## Miura-ori geometric study

| Filename | Type |
|---|---|
| `Miuri-Ori_plan_angulos diferentes.pdf` | PDF |
| `Miuri-Ori_plan_angulos diferentes.jpg` | JPG |
| `Miuri-Ori_plan_angulos_diferentes.ai` | Adobe Illustrator |

## Miura-ori 3D model

| Filename | Type |
|---|---|
| `MiuriOri_7x4.f3d` | Autodesk Fusion 360 |
| `MiuriOri_7x4_3D_v6.stl` | STL |
| `MiuriOri_7x4.obj` | OBJ |

## Miura-ori crease pattern

| Filename | Type |
|---|---|
| `MiuraOri_7x4.dxf` | DXF |
| `MiuraOri_7x4.pdf` | PDF |

## Kresling

| Filename | Type |
|---|---|
| `Kresling_6gon_A_and_B_TwoInchEdgeLength.dxf` | DXF |
| `KreslingArrayCreasePattern.dxf` | DXF |
| `KreslingArrayCreasePattern1.dxf` | DXF |
| `KreslingArrayCreasePattern1.studio3` | Studio 3 |

## Miura Alphabet

| Filename | Type |
|---|---|
| `Miura-Ori-Alphabet.f3d` | Autodesk Fusion 360 |

---

# Digital Fabrication

The geometric and CAD studies were complemented by physical prototyping.

Miura-ori structures were fabricated using different manufacturing
approaches, including:

- laser cutting and scoring of high-grammage paper;
- laser processing of polypropylene sheets;
- FDM 3D printing of Miura cells;
- FDM 3D printing of larger Miura structures.

These prototypes were used to investigate the transition from ideal geometric
models to physical objects.

Relevant considerations include:

- finite material thickness;
- fold realization;
- assembly;
- geometric continuity;
- manufacturing tolerances;
- repeatability of the unit cells.

The fabricated specimens are interpreted primarily as **geometric and
fabricability prototypes**.

---

# Origami-Inspired Metamaterials

Origami provides a useful design language for mechanical metamaterials because
the global behavior of a structure can be strongly influenced by the geometry
and connectivity of its repeating units.

In this context, the MetaOrigami project investigates a design hierarchy of
the form:

```text
          LOCAL SCALE

        Origami cell
             │
             ▼
     geometric parameters
             │
             ▼
       repeated modules

             │
             ▼

         GLOBAL SCALE

       meta-structure
             │
             ▼
      prescribed geometry
             │
             ▼
      reconfiguration
```

The Miura-ori and Kresling studies provide two complementary examples.

### Miura-ori

A predominantly planar periodic architecture characterized by strongly coupled
folding of repeated parallelogram-like facets.

### Kresling

A cylindrical triangulated architecture characterized by coupled axial and
torsional deformation.

Together they illustrate how different crease geometries can generate very
different classes of reconfigurable structures.

---

# Repository Structure

```text
MetaOrigami/
│
├── README.md
│
├── Miura-Ori-Alphabet.f3d
│
├── Kresling_6gon_A_and_B_TwoInchEdgeLength.dxf
├── KreslingArrayCreasePattern.dxf
├── KreslingArrayCreasePattern1.dxf
├── KreslingArrayCreasePattern1.studio3
│
├── EstudoCelulas/
│   │
│   ├── Miuri-Ori_plan_angulos diferentes.pdf
│   ├── Miuri-Ori_plan_angulos diferentes.jpg
│   └── Miuri-Ori_plan_angulos_diferentes.ai
│
└── FusionGeometries/
    │
    ├── Modelo_3D/
    │   │
    │   ├── GuiaArquivos3D.gdoc
    │   │
    │   └── MiuriOri/
    │       ├── MiuriOri_7x4.f3d
    │       ├── MiuriOri_7x4_3D_v6.stl
    │       └── MiuriOri_7x4.obj
    │
    └── Modelo_dxf_dwg/
        │
        └── CreasePattern/
            └── MiuraOri/
                ├── MiuraOri_7x4.dxf
                └── MiuraOri_7x4.pdf
```

---

# Research Status

| Topic | Status |
|---|---|
| Miura-ori geometric study | Completed |
| Miura-ori cell and tessellation | Developed |
| Miura-ori parametric CAD | Developed |
| Miura-ori 7 × 4 3D model | Available |
| Miura-ori DXF crease pattern | Available |
| Miura-ori physical prototypes | Produced |
| Miura geometric alphabet | Developed |
| Kresling geometric study | Exploratory |
| Kresling crease-pattern studies | Available |
| Kresling parametric closure | Under investigation |

---

# Authors

### Ana Beatriz Alencar Dias

Undergraduate Researcher  
Industrial Design  
**Universidade Federal do Rio de Janeiro — UFRJ**

### Americo Cunha Jr

Research Advisor  
**Laboratório Nacional de Computação Científica — LNCC**  
**Universidade do Estado do Rio de Janeiro — UERJ**

---

# Institutional Context

The project was developed as undergraduate research connecting:

- **Industrial Design**
- **Applied and Computational Mathematics**
- **Computational Geometry**
- **Digital Fabrication**
- **Origami Engineering**

The research activities involve the **Universidade Federal do Rio de Janeiro
(UFRJ)** and the **Laboratório Nacional de Computação Científica (LNCC)**,
with undergraduate research support associated with **FAPERJ**.

---

# Citation

If you use material from this repository in academic work, please cite the
project as:

> **A. B. A. Dias and A. Cunha Jr**,  
> *MetaOrigami: Origami-Inspired Meta-Structures, Parametric CAD and Digital
> Fabrication*, GitHub repository, 2026.

BibTeX:

```bibtex
@misc{DiasCunha2026MetaOrigami,
    author       = {A. B. A. Dias and A. Cunha Jr},
    title        = {MetaOrigami: Origami-Inspired Meta-Structures, Parametric CAD and Digital Fabrication},
    year         = {2026},
    howpublished = {GitHub repository}
}
```

---

# Contact

For questions about the project or research collaboration:

**Americo Cunha Jr**

Laboratório Nacional de Computação Científica — LNCC

---

<div align="center">

### MetaOrigami

**Geometry · Origami · CAD · Meta-Structures · Digital Fabrication**

2026

</div>

