# MIDGL

**MIDGL: Multimodal Dynamic Graph Learning for Spatial Domain Identification in Spatial Transcriptomics**

This repository provides the official implementation of **MIDGL**, a multimodal dynamic graph learning framework for spatial domain identification in spatial transcriptomics (ST).

> **Code availability:** The source code and experimental configurations will be publicly released upon acceptance of the corresponding paper.

---

## Overview

Spatial transcriptomics (ST) enables the simultaneous characterization of gene expression and spatial organization within biological tissues. Identifying spatial domains from ST data is an important step toward understanding tissue architecture and cellular organization. However, this task remains challenging due to the high dimensionality of gene expression profiles, spatial heterogeneity, noise, and complex tissue structures.

Existing methods have increasingly incorporated spatial information and histological morphology to improve spatial domain identification. However, multimodal approaches commonly rely on pre-constructed or fixed spatial graphs, which may limit their ability to adapt the underlying spatial relationships during representation learning.

To address these challenges, we propose **MIDGL**, a **Multimodal Dynamic Graph Learning** framework for spatial domain identification in spatial transcriptomics. MIDGL integrates complementary information from transcriptomic profiles, spatial organization, and tissue morphology while dynamically learning spatial graph structures during representation learning.

The learned representations are subsequently used to identify spatial domains with improved spatial coherence and biological interpretability.

---

## Key Features

* **Multimodal representation learning**
  Integrates complementary transcriptomic, spatial, and morphological information for spatial domain identification.

* **Dynamic graph learning**
  Dynamically adapts graph relationships during representation learning instead of relying solely on a fixed pre-constructed spatial graph.

* **Spatially informative representations**
  Learns representations that capture both molecular characteristics and spatial organization of tissue.

* **Robust spatial domain identification**
  Designed to identify coherent spatial domains in tissues with complex spatial heterogeneity.

* **Comprehensive evaluation**
  Evaluated on multiple spatial transcriptomics datasets using quantitative metrics and biological/spatial analyses.

---

## Framework

The overall framework of MIDGL consists of multimodal feature extraction, dynamic graph learning, representation learning, and spatial domain identification.

The framework is designed to progressively learn informative representations while adapting spatial relationships according to the learned multimodal features.

<p align="center">
  <img src="figures/MIDGL_framework.png" width="850">
</p>

*Overview of the MIDGL framework. The figure will be added together with the public code release.*

---

## Datasets

MIDGL is evaluated on multiple spatial transcriptomics datasets, including mouse brain and human breast cancer datasets.

The experiments include datasets with different tissue structures and spatial organization, allowing the effectiveness of MIDGL to be evaluated under diverse biological conditions.

In particular, the experiments include:

* **Mouse brain spatial transcriptomics datasets**
* **Human breast cancer datasets**
* **HER2+ breast cancer tissue**
* **MVC dataset**
* **Multi-slice spatial transcriptomics data**, including integrated slices such as 151673–151676

Raw datasets are not included in this repository. Users should obtain the corresponding datasets from their original public sources and follow their respective data-use requirements.

Detailed preprocessing instructions and dataset configurations will be provided with the code release.

---

## Experimental Evaluation

We compare MIDGL with representative spatial domain identification methods from different methodological categories.

The evaluation considers both quantitative performance and biological/spatial interpretability.

### Quantitative evaluation

The experiments include commonly used clustering and spatial-domain evaluation metrics, such as:

* Adjusted Rand Index (ARI)
* Normalized Mutual Information (NMI)
* Silhouette Coefficient (SC)

### Spatial and biological evaluation

In addition to quantitative metrics, we evaluate the inferred domains through:

* Spatial domain visualization
* Comparison with manual/pathological annotations
* Marker-gene expression patterns
* Spatial organization of biologically meaningful tissue regions
* Multi-slice representation visualization

These analyses are used to assess whether the learned domains correspond to meaningful biological structures rather than merely forming compact clusters in the learned feature space.

---

## Results

MIDGL achieves competitive or improved performance across multiple spatial transcriptomics datasets and produces spatial domains with coherent tissue boundaries.

The experimental results demonstrate that dynamically adapting graph relationships during multimodal representation learning can better capture the complex spatial organization of biological tissues.

Representative spatial clustering results and quantitative comparisons will be included in this repository after the public code release.

<p align="center">
  <img src="figures/MIDGL_results.png" width="850">
</p>

*Representative results will be added after the code release.*

---

## Code Availability

The source code is **not publicly released at this stage**.

The complete implementation, preprocessing scripts, experimental configurations, and instructions for reproducing the results reported in the paper will be released after the paper is accepted for publication.

Once released, this repository will include:

```text
MIDGL/
├── README.md
├── requirements.txt
├── data/
├── model/
├── preprocessing/
├── experiments/
├── utils/
└── ...
```

---

## Citation

If you find MIDGL useful in your research, please consider citing our paper:

```bibtex
@article{zhang2026midgl,
  title   = {MIDGL: Multimodal Dynamic Graph Learning for Spatial Domain Identification in Spatial Transcriptomics},
  author  = {Zhang Huanqi and Wang Zhaowei and Wang Yuangang and Duan Xiaodong and Dai Qiguo},
  journal = {Neurocomputing},
  year    = {2026}
}
```

> The citation information will be updated with the final bibliographic details after publication.

---

## Contact

For questions, suggestions, or issues related to MIDGL, please open an issue in this repository after the code release.

For correspondence:

**Huanqi Zhang**
Email: `<202412054042@dlnu.edu.cn>`

---

## License

The license information will be provided together with the public code release.
