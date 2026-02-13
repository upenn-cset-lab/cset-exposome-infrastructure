# C-SET Exposome Infrastructure

Scalable spatiotemporal data pipelines and modeling infrastructure for transplant exposome research, developed by the Center for Systems Epidemiology and Transplant Exposomics (C-SET), Penn Medicine.
## Scientific Scope

C-SET integrates environmental exposure science, biostatistics, systems epidemiology, and causal inference to understand how multidimensional environmental exposures influence solid organ transplant outcomes.

This repository focuses on:

- Spatiotemporal exposure assignment
- Longitudinal transplant dataset construction
- Advanced biostatistical modeling frameworks
- Distributed lag and time-varying exposure-response modeling
- Machine learning and high-dimensional data integration
- Scalable high-performance computing (HPC) workflows
- Reproducible Standard Analysis File (SAF) generation

## Core Components

### Data Infrastructure

#### Clinical Transplant Data
- Registry: USRDS (Core, UNOS)
- Claims: CMS Claims
- EHR: Epic COSMOS
- ICD-10 diagnostic groupings (e.g., infection, cardiovascular disease)

#### Environmental Exposure Data
- USHAP (PM2.5 and air pollution metrics)
- PRISM (temperature and climate variables)

#### Spatial and Geocoding Resources
- US Census Bureau ZCTA shapefiles and Gazetteer files
- HRSA ZIP–ZCTA crosswalk
- HUD ZIP–County crosswalk

#### Composite and Vulnerability Indices
- CVI and related contextual indices

### Pipelines
- Exposure extraction and spatial linkage
- USRDS Longitudinal dataset construction
- Modeling workflows (GAMs, distributed lag models, Bayesian hierarchical models, causal inference frameworks)
- HPC batch configuration templates

### Reproducibility Principles
- Secure data storage in institutional platforms
- Fully annotated and modular code
- End-to-end reproducible workflows
- Clear documentation and version control

---

© C-SET Lab
