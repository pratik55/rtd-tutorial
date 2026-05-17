# Module Name: `whifun_functions/whifun_qc_coreg_slover.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_COREG_SLOVER Creates a quality control image using SLover. WHIFUN_QC_COREG_SLOVER(image_1_path, image_2_path, out_image_path, slover_slices, slover_contour_range, slover_view) generates a quality control image to visually inspect the alignment of two neuroimaging files, using a specialized function (`whifun_slover`) for creating overlaid slices. This function is an alternative to `spm_check_registration` for creating a quality control image. It sets up an invisible SPM figure, calls a helper function (`whifun_slover`) to perform the visualization with specific parameters, and then ex
  - Internal calls detected: `whifun_slover`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `whifun_qc_coreg_slover()`

### Syntax
```matlab
function whifun_qc_coreg_slover(image_1_path,image_2_path,out_image_path,slover_slices,slover_contour_range,slover_view)
```
Defined at source line `1`.

### Description
WHIFUN_QC_COREG_SLOVER Creates a quality control image using SLover. WHIFUN_QC_COREG_SLOVER(image_1_path, image_2_path, out_image_path, slover_slices, slover_contour_range, slover_view) generates a quality control image to visually inspect the alignment of two neuroimaging files, using a specialized function (`whifun_slover`) for creating overlaid slices. This function is an alternative to `spm_check_registration` for creating a quality control image. It sets up an invisible SPM figure, calls a helper function (`whifun_slover`) to perform the visualization with specific parameters, and then exports the resulting figure to a file. The visual output will show one image (e.g., anatomical) as a

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `image_1_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `image_2_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_image_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_slover`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_qc_coreg.m:1/whifun_qc_coreg`, `whifun_functions/whifun_qc_csf_mask_alignment.m:1/whifun_qc_csf_mask_alignment`, `whifun_functions/whifun_qc_final_func_MNI.m:1/whifun_qc_final_func_MNI`, `whifun_functions/whifun_qc_initial_align_check.m:80/store_ortho_slover_images`, `whifun_functions/whifun_qc_normalize.m:1/whifun_qc_normalize`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_slover`
- Related callers: `whifun_functions/whifun_qc_coreg.m:1/whifun_qc_coreg`, `whifun_functions/whifun_qc_csf_mask_alignment.m:1/whifun_qc_csf_mask_alignment`, `whifun_functions/whifun_qc_final_func_MNI.m:1/whifun_qc_final_func_MNI`, `whifun_functions/whifun_qc_initial_align_check.m:80/store_ortho_slover_images`, `whifun_functions/whifun_qc_normalize.m:1/whifun_qc_normalize`
