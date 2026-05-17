# Module Name: `whifun_functions/whifun_qc_seed_corr.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_QC_SEED_CORR Generates quality control images for seed-based functional connectivity. WHIFUN_QC_SEED_CORR(out_folder, final_func_MNI, name, thresh, rad, slover_slices_mni, slover_view, over_write, func_mask_MNI) creates a visual quality control report to assess the quality of a subject's functional data by performing a simple seed-to-voxel correlation. The function calculates the correlation map for three standard functional networks: 1. **Default Mode Network (DMN)**: Seeded in the left Posterior Cingulate Cortex (PCC). 2. **Visual Network**: Seeded in the right visual cortex. 3. **Aud
  - Internal calls detected: `whifun_create_file`, `whifun_seed_corr_qc_plot`
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## `whifun_qc_seed_corr()`

### Syntax
```matlab
function whifun_qc_seed_corr(out_folder,final_func_MNI,name,thresh,rad,slover_slices_mni,slover_view,over_write,func_mask_MNI)
```
Defined at source line `1`.

### Description
WHIFUN_QC_SEED_CORR Generates quality control images for seed-based functional connectivity. WHIFUN_QC_SEED_CORR(out_folder, final_func_MNI, name, thresh, rad, slover_slices_mni, slover_view, over_write, func_mask_MNI) creates a visual quality control report to assess the quality of a subject's functional data by performing a simple seed-to-voxel correlation. The function calculates the correlation map for three standard functional networks: 1. **Default Mode Network (DMN)**: Seeded in the left Posterior Cingulate Cortex (PCC). 2. **Visual Network**: Seeded in the right visual cortex. 3. **Auditory Network**: Seeded in the left auditory cortex. For each network, the function performs the fol

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `final_func_MNI` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `thresh` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `rad` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices_mni` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_mask_MNI` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_seed_corr_qc_plot`
- **External Dependencies:** SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_seed_corr_qc_plot`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`
