# Aquatic Invasive Species Modeling and Metabarcoding Framework

**Integrated research and training workflows for aquatic invasive species risk assessment and environmental DNA biodiversity analysis in the Upper Mississippi River System (UMRS).**

**Project status:** Under active development

---

## Overview

This repository contains two complementary computational pipelines developed to support aquatic invasive species (AIS) research, risk assessment, and biological data generation within the Upper Mississippi River System (UMRS). Together, these tools provide a framework for evaluating aquatic invasive plant risks, generating spatial predictions of potential invasion hotspots, and expanding the biological data available to inform future modeling efforts.

The **ensemble modeling pipeline** integrates species occurrence records, environmental predictors, and geospatial datasets to estimate patterns of aquatic invasive plant introduction and establishment risk across the UMRS. Implemented through Python-based Jupyter notebooks and Google Earth Engine (GEE), the framework supports the development, evaluation, and visualization of ensemble model predictions. A central application is a hands-on workshop in which participants explore the modeling framework, examine environmental and ecological drivers of invasion risk, and generate spatial heatmaps highlighting areas with potentially elevated risk. The workflow is designed to facilitate practical engagement with invasion risk modeling while providing opportunities to investigate the influence of different predictor groups, model configurations, and environmental conditions on predicted risk.

The **metabarcoding pipeline** provides a complementary molecular ecology workflow for processing and evaluating environmental DNA (eDNA) metabarcoding data. Built around Snakemake and QIIME 2, the pipeline supports sequence processing, amplicon sequence variant (ASV) generation, taxonomic assignment, and downstream evaluation and synthesis. Particular emphasis is placed on quantifying how bioinformatic processing decisions, including sequence filtering, denoising, and taxonomic identification parameters, influence resulting biodiversity assessments. This evaluation framework provides a reproducible approach for assessing the sensitivity of metabarcoding results to analytical choices.

Although independently executable, the two pipelines are intended to support an interconnected research program. Metabarcoding-derived aquatic plant occurrence information can provide additional biological observations for future model development, evaluation, and refinement, potentially improving understanding of invasion patterns and spatial risk across the UMRS. By combining molecular biodiversity assessment with spatially explicit ecological modeling, this repository supports reproducible research, applied training, and the continued development of data-driven approaches for aquatic invasive species early detection and management.

---

## Repository Organization

The repository is organized into two independently maintained analytical pipelines.

| Directory | Description |
|---|---|
| `metabarcoding/` | eDNA metabarcoding sequence processing, taxonomic assignment, methodological evaluation, and synthesis |
| `modeling/` | Ensemble modeling, geospatial processing, spatial prediction, and workshop materials |
| `docs/` | Project-level documentation, architecture, and reproducibility guidance |

Each pipeline will maintain its own documentation, configuration files, software dependencies, and execution instructions.

## Pipelines

### 1. eDNA Metabarcoding Pipeline

**Location:** `metabarcoding/`

A reproducible workflow for processing and evaluating environmental DNA metabarcoding data.

Primary components include:

- Sequence quality assessment and processing.
- Read filtering and denoising using QIIME 2 and DADA2.
- Amplicon sequence variant (ASV) generation.
- Taxonomic assignment and reference database evaluation.
- Sensitivity analyses examining the effects of bioinformatic parameters and filtering decisions.
- Post-processing, evaluation, and visualization of biodiversity results.

**Workflow framework:** Snakemake / QIIME 2 / Python

See [`metabarcoding/README.md`](metabarcoding/README.md) for pipeline-specific documentation.

### 2. Ensemble Invasion Risk Modeling Pipeline

**Location:** `modeling/`

A geospatial modeling framework for evaluating and visualizing aquatic invasive plant introduction and establishment risk across the UMRS.

Primary components include:

- Integration of species occurrence and environmental predictor datasets.
- Geospatial data preparation and processing.
- Ensemble model development and evaluation.
- Assessment of environmental and ecological drivers of invasion risk.
- Generation of spatial predictions and risk heatmaps.
- Hands-on workshop materials and instructional workflows.

**Workflow framework:** Python / Jupyter Notebooks / Google Earth Engine

The modeling pipeline is associated with a separate Google Earth Engine code repository and its supporting geospatial resources. Dependencies and external resources will be documented in the modeling-specific README.

See [`modeling/README.md`](modeling/README.md) for pipeline-specific documentation.

---

## Getting Started

Both pipelines are maintained as independent workflows. Users should consult the corresponding pipeline documentation for installation requirements, software dependencies, configuration instructions, input data requirements, and execution procedures.

Pipeline-specific installation and execution instructions will be added as development progresses.

## Data and Reproducibility

This repository is intended to support transparent and reproducible research. Software environments, analytical configurations, processing parameters, and relevant workflow documentation will be maintained alongside the respective pipelines.

Large datasets, raw sequencing files, intermediate analytical outputs, and externally hosted geospatial resources may be maintained outside the repository. Instructions for accessing required external data and resources will be provided where appropriate.

Users should consult the pipeline-specific documentation before attempting to reproduce analytical results.

## Development Status

Both pipelines are under active development.

The metabarcoding pipeline is undergoing initial evaluation and development of its methodological assessment, synthesis, and visualization components. The ensemble modeling pipeline is being maintained as a research and training framework, with an emphasis on reproducible spatial risk assessment and workshop applications.

Features, dependencies, documentation, and execution procedures may change as development and evaluation continue.

## Citation

A formal software citation will be provided through the repository's `CITATION.cff` metadata file once project authorship, attribution, and release information have been finalized.

If you use either pipeline in research, presentations, or other applications, please cite the associated software release and relevant publications where available.

## Funding and Acknowledgments

Development of these computational workflows is supported in part by the U.S. Geological Survey (USGS).

Additional project collaborators, institutional affiliations, funding acknowledgments, and relevant contributions will be documented as the repository develops.

## License

Licensing and software distribution terms will be established following confirmation of applicable institutional and project requirements.

---

**Maintained by:** [Project authors and contributors to be added]

**Project affiliation:** [Institutional affiliation to be added]

**Repository:** [GitHub repository URL to be added]
