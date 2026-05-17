# Module Name: `whifun_functions/whifun_qc_normalize.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_NORMALIZE Generates quality control figures for normalization. WHIFUN_QC_NORMALIZE(out_folder, Subj_list_1, template_path, slover_slices_mni, slover_contour_range_mni, slover_view, over_write) creates a visual report to assess the quality of spatial normalization. The function checks if the subject's functional data has been accurately warped into a standard template space (e.g., MNI). The function performs three main checks: 1. **Orthoslice Alignment**: It generates an SPM `check_registration` plot. It uses the first volume of the normalized functional image as the underlay and a st
  - Internal calls detected: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`, `whifun_ts_mask_qc`, `whifun_ts_qc`
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## `whifun_qc_normalize()`

### Syntax
```matlab
function whifun_qc_normalize(out_folder,Subj_list_1,template_path,slover_slices_mni,slover_contour_range_mni,slover_view,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_QC_NORMALIZE Generates quality control figures for normalization. WHIFUN_QC_NORMALIZE(out_folder, Subj_list_1, template_path, slover_slices_mni, slover_contour_range_mni, slover_view, over_write) creates a visual report to assess the quality of spatial normalization. The function checks if the subject's functional data has been accurately warped into a standard template space (e.g., MNI). The function performs three main checks: 1. **Orthoslice Alignment**: It generates an SPM `check_registration` plot. It uses the first volume of the normalized functional image as the underlay and a standard MNI template as the overlay. This provides a quick visual check of the alignment. 2. **SLover

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `template_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices_mni` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range_mni` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`, `whifun_ts_mask_qc`, `whifun_ts_qc`
- **External Dependencies:** SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`, `whifun_ts_mask_qc`, `whifun_ts_qc`
