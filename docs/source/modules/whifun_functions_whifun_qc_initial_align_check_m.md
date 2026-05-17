# Module Name: `whifun_functions/whifun_qc_initial_align_check.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_INITIAL_ALIGN_CHECK Creates quality control images for initial data alignment. WHIFUN_QC_INITIAL_ALIGN_CHECK(out_folder, template_path, Subj_list_1, slover_slices, slover_contour_range, slover_view, over_write) generates visual quality control reports to assess the initial alignment of a subject's functional and anatomical data to a standard MNI template. The function performs two main tasks: 1. **Anatomical Alignment Check**: It creates QC images comparing the subject's anatomical file to an MNI template. 2. **Functional Alignment Check**: It creates QC images comparing the first vo
  - Internal calls detected: `whifun_create_file`, `whifun_multiple_file_found`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `whifun_qc_initial_align_check()`

### Syntax
```matlab
function whifun_qc_initial_align_check(out_folder,template_path,Subj_list_1,slover_slices,slover_contour_range,slover_view,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_QC_INITIAL_ALIGN_CHECK Creates quality control images for initial data alignment. WHIFUN_QC_INITIAL_ALIGN_CHECK(out_folder, template_path, Subj_list_1, slover_slices, slover_contour_range, slover_view, over_write) generates visual quality control reports to assess the initial alignment of a subject's functional and anatomical data to a standard MNI template. The function performs two main tasks: 1. **Anatomical Alignment Check**: It creates QC images comparing the subject's anatomical file to an MNI template. 2. **Functional Alignment Check**: It creates QC images comparing the first volume of the subject's functional file to the same MNI template. For each alignment check, a helper f

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `template_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range` — MATLAB value inferred from source usage
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
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_multiple_file_found`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_multiple_file_found`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`

## `store_ortho_slover_images()`

### Syntax
```matlab
function store_ortho_slover_images(image_1_path,image_2_path,out_ortho_path,out_slover_path,slover_slices,slover_contour_range,slover_view,over_write)
```
Defined at source line `80`.

### Description
WHIFUN_QC_INITIAL_ALIGN_CHECK Creates quality control images for initial data alignment. WHIFUN_QC_INITIAL_ALIGN_CHECK(out_folder, template_path, Subj_list_1, slover_slices, slover_contour_range, slover_view, over_write) generates visual quality control reports to assess the initial alignment of a subject's functional and anatomical data to a standard MNI template. The function performs two main tasks: 1. **Anatomical Alignment Check**: It creates QC images comparing the subject's anatomical file to an MNI template. 2. **Functional Alignment Check**: It creates QC images comparing the first vo

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `image_1_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `image_2_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_ortho_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_slover_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range` — MATLAB value inferred from source usage
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
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`
- **External Dependencies:** SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`
