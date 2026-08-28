<div align="center">

# MetaOrigami

### Parametric CAD, digital fabrication and reconfigurable origami meta-structures

**Miura-ori · Kresling · Waterbomb · fabrication · geometric programming · metamaterials**

[![Project status](https://img.shields.io/badge/status-active-1f6feb)](https://github.com/americocunhajr/MetaOrigami)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-v0.1-2ea44f)](https://americocunhajr.github.io/MetaOrigami/)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/license-CC%20BY--SA%204.0-lightgrey)](https://creativecommons.org/licenses/by-sa/4.0/)

<img src="assets/images/hero_metaorigami.jpg" alt="MetaOrigami: Miura-ori models, prototypes and geometric alphabet" width="100%">

**Undergraduate research project on origami engineering, parametric geometry and digital prototyping.**

[Overview](#overview) · [Results](#main-results) · [Models](#models-and-files) · [Fabrication](#digital-fabrication) · [Gallery](#gallery) · [Roadmap](#roadmap) · [Website](#github-pages)

</div>

---

## Overview

**MetaOrigami** investigates how origami crease patterns can be translated into **parametric CAD models, reconfigurable structures and digitally fabricated prototypes**. The project focuses on the geometric rules that connect a local folding cell to the global shape and kinematics of a meta-structure.

The current work uses **Miura-ori** as the main reference geometry and extends the investigation to **Kresling** and **Waterbomb** patterns. The broader objective is to build a reusable library of models and fabrication procedures for research in **origami engineering, mechanical metamaterials, reconfigurable structures and morphological design**.

The project combines:

- geometric analysis of crease patterns and unit cells;
- parametric modeling in Autodesk Fusion 360;
- study of opening/closing kinematics and geometric compatibility;
- laser-cut fabrication in sheet materials;
- FDM 3D printing of cells and structures;
- exploration of complex shapes generated from repeated origami cells;
- open documentation and distribution of CAD/fabrication files.

> **Research stage.** This repository documents an undergraduate research project in active development. Some models are mature proof-of-concept implementations, while others remain exploratory and are explicitly identified as such.

## Main results

### 1. Parametric Miura-ori models

A parametric description of the Miura-ori cell was implemented in CAD to study the influence of geometric variables on the folded configuration. Different tessellation sizes, aspect ratios and folding configurations were explored, enabling the geometry to be modified without rebuilding the complete model.

<p align="center">
<img src="assets/images/miura_render.jpg" width="47%" alt="Rendered Miura-ori structure"> &nbsp;
<img src="assets/images/miura_tessellations.png" width="47%" alt="Miura-ori tessellations">
</p>

The model also provided a practical framework for identifying geometric limits associated with face interference, compactness and inversion of the expected configuration.

### 2. Miura-ori alphabet as a geometric proof of concept

A complete alphabet was constructed from Miura-ori-inspired modular cells. The purpose is not typography as an isolated design exercise: the alphabet acts as a **proof of concept for geometric programmability**, demonstrating that a repeated cell can be reorganized to generate complex global shapes while preserving a common construction logic.

<p align="center">
<img src="assets/images/miura_alphabet.png" width="92%" alt="Miura-ori alphabet proof of concept">
</p>

This experiment is relevant to the longer-term study of meta-structures in which **global form emerges from the controlled arrangement of local geometric units**.

### 3. Physical fabrication

Physical models were produced using more than one fabrication route. Miura-ori sheets were fabricated by **laser cutting and scoring** in high-grammage paper and polypropylene, while cells and spatial structures were also produced by **FDM 3D printing**.

<p align="center">
<img src="assets/images/prototipos_fisicos.jpeg" width="88%" alt="Physical origami prototypes produced during the project">
</p>

These prototypes are used to compare digital geometry with actual foldability, assembly constraints, material thickness effects and fabrication tolerances.

### 4. Kresling exploration

Kresling geometries were studied in parallel as a second family of deployable structures. The work exposed a more demanding parametric closure problem: changes in one geometric variable affect several coupled dimensions and angles. The current files therefore document **exploratory models and crease patterns**, rather than a fully validated parametric Kresling generator.

<p align="center">
<img src="assets/images/kresling_cad.png" width="72%" alt="Kresling CAD exploration">
</p>

This limitation is part of the research result because it identifies the mathematical relations that must be resolved before a robust parametric implementation can be obtained.

## Project status

| Work package | Status | Current output |
|---|---|---|
| Geometric foundations and CAD training | Completed | geometric studies, CAD workflow and documentation |
| Miura-ori cell and tessellations | Advanced | parametric CAD models and multiple configurations |
| Miura-ori kinematics | Advanced | opening/closing configurations and geometric limits |
| Laser-cut prototypes | Completed at proof-of-concept level | paper and polypropylene sheets |
| FDM prototypes | Completed at proof-of-concept level | printed cells and spatial structures |
| Complex-form demonstrator | Completed | Miura-ori alphabet |
| Kresling | In progress | exploratory CAD and crease-pattern files |
| Waterbomb | Next work package | systematic model and prototypes to be developed |
| Open website and repository | v0.1 | this repository and GitHub Pages structure |

## Models and files

The repository keeps research files separated from the website source.

```text
MetaOrigami/
│
├── README.md                     # GitHub repository landing page
├── CITATION.cff                  # citation metadata
├── LICENSE.md
├── DEPLOY.md                     # GitHub Pages instructions
│
├── assets/
│   └── images/                   # images used in the repository README
│
├── models/
│   ├── miura_ori/                # F3D, STL, DXF, OBJ and reference geometry
│   ├── kresling/                 # exploratory crease-pattern files
│   └── waterbomb/                # next work package
│
├── documentation/                # fabrication, parameters and project notes
│
└── docs/                         # GitHub Pages website
    ├── index.md
    ├── models.md
    ├── fabrication.md
    ├── gallery.md
    ├── roadmap.md
    ├── about.md
    ├── _config.yml
    └── assets/
```

### Miura-ori

Available formats include:

- Autodesk Fusion 360 (`.f3d`)
- STL (`.stl`)
- DXF (`.dxf`)
- OBJ (`.obj`)
- DWG reference geometry (`.dwg`)

See [`models/miura_ori/`](models/miura_ori/).

### Kresling

The Kresling folder currently contains exploratory crease-pattern files used during the geometric study. They should not yet be interpreted as a validated parametric library.

See [`models/kresling/`](models/kresling/).

### Waterbomb

The Waterbomb package is intentionally reserved as the next stage of the project. It will contain the parametric cell, tessellations, fabrication files and physical prototypes as they are completed.

See [`models/waterbomb/`](models/waterbomb/).

## Digital fabrication

Two fabrication strategies are currently represented.

### Laser cutting

Miura-ori sheets were produced in:

- high-grammage paper;
- polypropylene sheet.

The fabrication workflow includes preparation of the planar crease pattern, definition of cutting/scoring layers, adjustment of laser parameters and manual verification of foldability.

### FDM 3D printing

Cells and assembled structures were produced by FDM printing to explore:

- finite panel thickness;
- geometric continuity;
- repeatability of unit cells;
- assembly and handling;
- translation from ideal zero-thickness geometry to physical specimens.

See [`documentation/guia_fabricacao.md`](documentation/guia_fabricacao.md) for the initial fabrication notes.

## Gallery

<table>
<tr>
<td width="50%"><img src="assets/images/miura_render.jpg" alt="Miura render"><br><b>Parametric Miura-ori</b></td>
<td width="50%"><img src="assets/images/miura_tessellations.png" alt="Miura tessellations"><br><b>Geometric variations</b></td>
</tr>
<tr>
<td width="50%"><img src="assets/images/miura_alphabet.png" alt="Miura alphabet"><br><b>Complex-form proof of concept</b></td>
<td width="50%"><img src="assets/images/prototipos_fisicos.jpeg" alt="Physical prototypes"><br><b>Physical prototypes</b></td>
</tr>
</table>

## Future direction: origami concepts for medical devices

A subsequent stage will broaden the geometric library and evaluate origami architectures according to functional requirements such as **deployability, radial expansion, compact storage, conformability and controlled reconfiguration**. One possible application direction is the conceptual design of medical devices.

<p align="center">
<img src="assets/images/medical_device_concepts.png" width="88%" alt="Illustrative map of origami-inspired medical device concepts">
</p>

The figure is an **illustrative concept map**, not a set of validated medical devices. The intended workflow is to compare candidate origami geometries, select one promising configuration, establish design requirements, create a CAD model and fabricate a proof-of-concept prototype.

## Roadmap

- [x] Miura-ori geometric study
- [x] Parametric Miura-ori CAD implementation
- [x] Multiple Miura-ori tessellations
- [x] Laser-cut proof-of-concept specimens
- [x] FDM printed cells and structures
- [x] Complex-form demonstrator using Miura modules
- [x] Initial Kresling investigation
- [ ] Complete Waterbomb geometric study
- [ ] Implement Waterbomb parametric CAD model
- [ ] Fabricate Waterbomb specimens
- [ ] Consolidate Kresling closure relations
- [ ] Standardize fabrication/experimental records
- [ ] Compare origami geometries for a selected functional application
- [ ] Design and fabricate one application-oriented proof of concept

## GitHub Pages

A first website version is included in [`docs/`](docs/). It uses the **Cayman** GitHub Pages theme and can be published without an external web framework.

To publish:

1. Create the repository `MetaOrigami` on GitHub.
2. Upload/commit the contents of this folder.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch **main** and folder **/docs**.
6. Save and wait for GitHub Pages to build the site.

The default URL will be:

```text
https://americocunhajr.github.io/MetaOrigami/
```

For a custom domain, `metaorigami.org` is a concise option if available. Detailed instructions are in [`DEPLOY.md`](DEPLOY.md).

## Documentation

Initial technical notes are stored under [`documentation/`](documentation/), including:

- geometric requirements and parameters;
- Miura-ori storyboard;
- fabrication guide;
- fabrication data sheet;
- project deliverable matrix;
- extended abstract draft.

These documents are expected to evolve as the CAD library and experimental procedures become more mature.

## Authors

- **Ana Beatriz Alencar Dias** — undergraduate researcher, Design Industrial, Universidade Federal do Rio de Janeiro (UFRJ)
- **Americo Cunha Jr** — advisor, Laboratório Nacional de Computação Científica (LNCC) / Universidade do Estado do Rio de Janeiro (UERJ)

## How to cite

Until a formal publication or repository DOI is available, cite the project as:

> A. B. A. Dias and A. Cunha Jr, **MetaOrigami: Parametric CAD, Digital Fabrication and Reconfigurable Origami Meta-structures**, GitHub repository, 2026.

A machine-readable citation file is provided in [`CITATION.cff`](CITATION.cff).

## License

Unless otherwise indicated, original documentation and project-generated media in this repository are distributed under the **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** license. CAD files derived from external sources must retain the license and attribution of their respective sources.

See [`LICENSE.md`](LICENSE.md).

## Funding and institutional context

This work was developed as an undergraduate research project with support associated with **FAPERJ** and research activities at **LNCC**, in connection with the student's undergraduate training at **UFRJ**.

## Contact

For questions about the project, repository or research collaboration:

- **Americo Cunha Jr** — americo@lncc.br

---

<div align="center">
<sub>MetaOrigami · first public repository/site version · 2026</sub>
</div>
