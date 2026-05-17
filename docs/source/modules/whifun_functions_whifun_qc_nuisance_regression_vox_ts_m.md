# Module Name: `whifun_functions/whifun_qc_nuisance_regression_vox_ts.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_NUISANCE_REGRESSION_VOX_TS Generates quality control figures for nuisance regression. WHIFUN_QC_NUISANCE_REGRESSION_VOX_TS(out_folder1, Subj_list_1, ...) creates visual quality control reports to assess the effectiveness of nuisance regression. The function focuses on time series plots and mask visualizations. The function performs the following steps: 1. **Check Existence**: It checks if the before- and after-regression time series plots already exist and, based on the `over_write` flag, either skips or generates new ones. It also creates the necessary output directories. 2. **Time 
  - Internal calls detected: `whifun_create_file`, `whifun_ts_mask_qc`, `whifun_ts_qc`
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## Function: `whifun_qc_nuisance_regression_vox_ts()`
- **Signature & Definition:** `function whifun_qc_nuisance_regression_vox_ts(out_folder1,Subj_list_1,slover_slices_ss,slover_contour_range_ss,slover_view,over_write)` (line 1)
- **Scientific Theory & Formulas:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_QC_NUISANCE_REGRESSION_VOX_TS Generates quality control figures for nuisance regression. WHIFUN_QC_NUISANCE_REGRESSION_VOX_TS(out_folder1, Subj_list_1, ...) creates visual quality control reports to assess the effectiveness of nuisance regression. The function focuses on time series plots and mask visualizations. The function performs the following steps: 1. **Check Existence**: It checks if the before- and after-regression time series plots already exist and, based on the `over_write` flag, either skips or generates new ones. It also creates the necessary output directories. 2. **Time Series Plots**: It calls a helper function `whifun_ts_qc` to generate time series plots of key brain
- **Arguments:**
  - `out_folder1` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_slices_ss` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_contour_range_ss` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_view` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_create_file`, `whifun_ts_mask_qc`, `whifun_ts_qc`
  - External: SLover/MarsBaR-style visualization helpers
  - Called By: `whifun_functions/whifun_qc.m:1/whifun_qc`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.
