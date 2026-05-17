# Module Name: `whifun_functions/whifun_seed_corr_qc_plot.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SEED_CORR_QC_PLOT Computes seed-based functional connectivity (FC) and generates a quality control (QC) visualization using the Slover tool. WHIFUN_SEED_CORR_QC_PLOT(OUTPUT_PATH, FUNC_PATH, SEED, RAD, SEED_COR_OUTPUT_PATH, THRESH, SLICES_MNI, VIEW, MASK) This function first calculates the seed-to-voxel correlation map for a given seed location. It then creates two temporary thresholded versions of the correlation map and visualizes them simultaneously using Slover (e.g., one for positive correlation, one for negative) on top of the structural image for QC purposes. The temporary files a
  - Internal calls detected: `whifun_seed_corr`, `whifun_slover`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## Function: `whifun_seed_corr_qc_plot()`
- **Signature & Definition:** `function whifun_seed_corr_qc_plot(output_path,func_path,seed,rad,seed_cor_output_path,thresh,slover_slices_mni,slover_view,mask)` (line 1)
- **Scientific Theory & Formulas:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_SEED_CORR_QC_PLOT Computes seed-based functional connectivity (FC) and generates a quality control (QC) visualization using the Slover tool. WHIFUN_SEED_CORR_QC_PLOT(OUTPUT_PATH, FUNC_PATH, SEED, RAD, SEED_COR_OUTPUT_PATH, THRESH, SLICES_MNI, VIEW, MASK) This function first calculates the seed-to-voxel correlation map for a given seed location. It then creates two temporary thresholded versions of the correlation map and visualizes them simultaneously using Slover (e.g., one for positive correlation, one for negative) on top of the structural image for QC purposes. The temporary files are deleted after plotting. Input Arguments: OUTPUT_PATH - Full path to save the final QC plot graphi
- **Arguments:**
  - `output_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `func_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `seed` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `rad` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `seed_cor_output_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `thresh` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_slices_mni` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_view` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mask` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_seed_corr`, `whifun_slover`
  - External: SPM12, SLover/MarsBaR-style visualization helpers
  - Called By: `whifun_functions/whifun_qc_seed_corr.m:1/whifun_qc_seed_corr`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.
