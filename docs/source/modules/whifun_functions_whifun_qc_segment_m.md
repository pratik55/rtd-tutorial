# Module Name: `whifun_functions/whifun_qc_segment.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_SEGMENT Generates quality control images for anatomical segmentation. WHIFUN_QC_SEGMENT(...) creates a visual report to assess the quality of the anatomical image segmentation. The function can generate two types of reports, one in the subject's native space and one in MNI space, depending on the input paths. The function performs the following steps: 1. **SPM Orthoslice Plot**: It creates a plot showing a reference image (`ref`) with overlaid contours of the segmented Gray Matter (GM), White Matter (WM), and Cerebrospinal Fluid (CSF). This provides a visual check of how well the seg
  - Internal calls detected: `whifun_create_file`, `whifun_create_seg_overlaps`, `whifun_slover`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `whifun_qc_segment()`

### Syntax
```matlab
function whifun_qc_segment(out_folder,name,ref,GM_path,WM_path,CSF_path,slover_slices,slover_contour_range,slover_view,space_name,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_QC_SEGMENT Generates quality control images for anatomical segmentation. WHIFUN_QC_SEGMENT(...) creates a visual report to assess the quality of the anatomical image segmentation. The function can generate two types of reports, one in the subject's native space and one in MNI space, depending on the input paths. The function performs the following steps: 1. **SPM Orthoslice Plot**: It creates a plot showing a reference image (`ref`) with overlaid contours of the segmented Gray Matter (GM), White Matter (WM), and Cerebrospinal Fluid (CSF). This provides a visual check of how well the segmentation process worked. 2. **SLover Plot**: It uses `whifun_slover` to display the segmented tissu

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `ref` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `GM_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `CSF_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `space_name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_create_seg_overlaps`, `whifun_slover`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_create_seg_overlaps`, `whifun_slover`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`
