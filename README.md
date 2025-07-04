<!--
Copyright (C) 2024 Roberto Rossini <roberros@uio.no>

SPDX-License-Identifier: CC0-1.0
-->

# Roberto Rossini – Scientific Software Developer & Bioinformatics Researcher

As a **scientific software developer** and **postdoctoral researcher in bioinformatics** at the University of Oslo, I design and build high-performance computational tools to solve complex problems in genomics and model the 3D genome organization.

I develop and maintain several **open-source tools**, primarily written in modern **C++** and **Python**, for:

- Hi-C and multi-omics data processing
- Modeling of the 3D genome structure
- Bioinformatics workflows for reproducible analysis
- CLI tools and libraries for large-scale genomics

When it comes to bioinformatics tools, I deeply care about:

- **Performance** — through efficient algorithms, parallelism, and modern systems programming
- **Correctness** — via rigorous testing and well-thought-out code architecture
- **Usability** — achieved with clear CLI design, intuitive APIs, and comprehensive documentation

## 🔬 Selected Projects

---

### [hictk](https://github.com/paulsengroup/hictk) • [hictkpy](https://github.com/paulsengroup/hictkpy) • [hictkR](https://github.com/paulsengroup/hictkR)

**A CLI and C++/Python/R library to efficiently handle data from Hi-C experiments**

- Designed to enable seamless operations on files in `.hic` and `cooler` formats, streamlining the analysis of 3D genomic data
- Convert `.hic` files to `.mcool` **up to 36x faster** than existing tools
- Zero-copy in-memory data sharing between C++ and Python/R using Arrow and Eigen
- Published in _OUP Bioinformatics_ (2024): [doi.org/10.1093/bioinformatics/btae408](https://doi.org/10.1093/bioinformatics/btae408)
- **Languages**: `C++17` (core), `Python`, `R`
- **Tech stack**: `Arrow`, `Conan`, `CMake`, `Docker`, `GitHub Actions`, `nanobind`, `OpenTelemetry`, `Rcpp`, `Sphinx`
- **Key Algorithms & Techniques**: Test-driven development, fuzzy testing, streaming algorithms, visitor and iterator patterns, multi-threading
- **Role**: Lead developer

---

<details>
<summary><strong>Click to see more</strong></summary>

### [MoDLE](https://github.com/paulsengroup/modle)

**A high-performance stochastic modeling of DNA loop extrusion interactions**

- Developed to simulate genome-wide loop extrusion in vertebrates, providing insights into chromatin dynamics relevant to gene regulation and disease mechanisms
- **Orders of magnitude faster** than traditional MD-based models: simulate loop extrusion on the human genome using consumer hardware in a few minutes
- Published in _Genome Biology_ (2022): [doi.org/10.1186/s13059-022-02815-7](https://doi.org/10.1186/s13059-022-02815-7)
- **Tech stack**: `C++17`, `Conan`, `CMake`, `Docker`, `GitHub Actions`
- **Key Algorithms & Techniques**: unit-testing, consumer-producer architecture, multi-threading, concurrent data structures
- **Role**: Lead developer

---

### [2022-mcf10a-cancer-progression](https://github.com/paulsengroup/2022-mcf10a-cancer-progression)

**3D Genome Analysis of Breast Cancer Progression in MCF10A and related cell lines**

- Full pipeline and analysis scripts for integrative Hi-C, ChIP-Seq, and RNA-Seq data
- Preprint available on bioRxiv (2023): [doi.org/10.1101/2023.11.26.568711](https://doi.org/10.1101/2023.11.26.568711)
- **Tools**: `Bash`, `Dash`, `Docker`, `Jupyter`, `Nextflow`, `Python`, `R`
- **Role**: Principal data scientist

---

### [StripePy](https://github.com/paulsengroup/StripePy)

**Detection of architectural stripes in Hi-C contact maps**

- Identifies structural features linked to active transcription and regulatory regions
- Format-agnostic and easy to use. Augments stripes with several descriptive statistics
- Published in _OUP Bioinformatics_ (2025): [doi.org/10.1093/bioinformatics/btaf351](https://doi.org/10.1093/bioinformatics/btaf351)
- **Language**: `Python`
- **Key Algorithms & Techniques**: unit-testing, multiprocessing, shared memory, asynchronous programming, structured logging
- **Role**: Primary code contributor. Provided inputs regarding the algorithm design

---

<details>
<summary><strong>Additional Tools & Workflows</strong> (Click to expand)</summary>

### Reproducible computational pipelines

The projects presented in this section aim to simplify and automate common bioinformatics analysis workflows using Nextflow and containers:

- [compress-nfcore-hic-output](https://github.com/robomics/compress-nfcore-hic-output) – Automates post-processing of nf-core Hi-C output files
- [chrom3d-nf](https://github.com/robomics/chrom3d-nf) – Reproducible Chrom3D modeling pipeline using Nextflow
- [call_tad_cliques](https://github.com/robomics/call_tad_cliques) – Identify TAD cliques from Hi-C data using an approach rooted in graph theory
- [generate_higlass_gene_track](https://github.com/robomics/generate_higlass_gene_track) – Prepares gene annotations for HiGlass visualization

All the above workflows are implemented using `Nextflow` (mainly using DSL2).\
Each repository is structured to leverage `GitHub Actions` and the `GitHub Container Registry (GHCR.io)` to build and host custom Docker images to enable reproducible data analysis without relying on third-party images.\
The code used in, and called by `Nextflow` processes is written using `Bash`, `Python`, and `R`.

</details>

---

## 🔧 Community & Ecosystem Contributions

In addition to major projects, I contribute to the broader bioinformatics software ecosystem:

- **Package maintenance**:
  - [Bioconda Recipes](https://github.com/bioconda/bioconda-recipes/issues?q=is%3Apr%20author%3Arobomics)
  - [Conan Center Index](https://github.com/conan-io/conan-center-index/pulls?q=is%3Apr+author%3Arobomics)
- **Bug fixes and patches**:
  - [cooler](https://github.com/open2c/cooler/issues?q=is%3Apr%20author%3Arobomics)
  - [Chrom3D](https://github.com/Chrom3D/Chrom3D/issues?q=is%3Apr%20author%3Arobomics)
  - [dcHiC](https://github.com/ay-lab/dcHiC/issues?q=is%3Apr%20author%3Arobomics)
  - [iced](https://github.com/hiclib/iced/issues?q=is%3Apr%20author%3Arobomics)
  - [nf-core/hic](https://github.com/nf-core/hic/issues?q=is%3Apr%20author%3Arobomics)
  - [stripenn](https://github.com/ysora/stripenn/issues?q=is%3Apr%20author%3Arobomics)
  - [libBigWig](https://github.com/dpryan79/libBigWig/issues?q=is%3Apr%20author%3Arobomics)

---

</details>

## 📫 Contact & Links

- 📍 Based in Oslo, Norway
- ✉️ [Work email](https://www.mn.uio.no/ibv/english/people/aca/roberros/)
- 🌐 [ORCID](https://orcid.org/0000-0003-3096-1470) | [LinkedIn](https://www.linkedin.com/in/robomics) | [Twitter](https://twitter.com/robomics)

Do not hesitate to connect with me on LinkedIn or reach out via email for collaborations or opportunities.

<!-- For full details, see my [CV (PDF)](TODO) or browse my repositories: [github.com/robomics](https://github.com/robomics?tab=repositories), [github.com/paulsengroup](https://github.com/paulsengroup). -->
