# Getting Started

# Scientific Documentation Skeleton: WhiFuN Toolbox

Static review date: 2026-05-16. This report was generated from repository source files without executing MATLAB, SPM, FSL, AFNI, or App Designer GUIs. Function signatures and call graphs are source-static, not runtime-profiler traces.

## Overview & Setup
- **High-level theory and purpose:** WhiFuN is a MATLAB toolbox for preprocessing BOLD fMRI, separating WM/GM tissue-informed signals, constructing WM and GM functional networks, extracting ROI/network average time series, computing FC matrices, visualizing network maps, and running FC association statistics.
- **Global external dependencies and required toolboxes:** MATLAB R2022a or later is recommended. Required MATLAB toolboxes from the README are Image Processing Toolbox, Signal Processing Toolbox, Statistics and Machine Learning Toolbox, and Bioinformatics Toolbox. Parallel Computing Toolbox is optional. The source also calls SPM12 extensively. Optional or alternate paths call FSL (`mcflirt`, `fsl_anat`, `epi_reg`, `applywarp`, `fslmaths`, `fast`, `bet`, `fsl_prepare_fieldmap`, `fugue`), AFNI (`align_epi_anat.py`, `3dcopy`), BrainNetViewer, SLover-like private visualization helpers, and `mexOMP` for K-SVD sparse coding.

## Documentation Map

- [Architecture](architecture)
- [Module Reference](modules/index)
- [Anomalies & Recommendations](anomalies)
