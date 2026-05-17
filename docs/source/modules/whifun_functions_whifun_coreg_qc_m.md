# Module Name: `whifun_functions/whifun_coreg_qc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COREG_QC Generates automated QC images for Coregistration. Author: Pratik Jain This function creates two types of visual checks: 1. Orthoslice View: A standard SPM-style three-pane check with contours. 2. Slice View: A detailed multi-slice layout using the 'slover' engine. INPUTS: name_ - String. Subject ID or session name. now_anat_path - Struct. Anatomical file info (from dir()). now_func_path - Struct. Functional file info (from dir()). slover_slices - Vector. Indices of slices to display. slover_contour_range - Vector. Range for contour levels (e.g., [0.5 0.5]). slover_view - String
  - Internal calls detected: `spm_check_registration_evalc`, `whifun_slover`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `whifun_coreg_qc()`

### Syntax
```matlab
function whifun_coreg_qc(name_,now_anat_path,now_func_path,slover_slices,slover_contour_range,slover_view,ss,quality_control_path)
```
Defined at source line `1`.

### Description
WHIFUN_COREG_QC Generates automated QC images for Coregistration. Author: Pratik Jain This function creates two types of visual checks: 1. Orthoslice View: A standard SPM-style three-pane check with contours. 2. Slice View: A detailed multi-slice layout using the 'slover' engine. INPUTS: name_ - String. Subject ID or session name. now_anat_path - Struct. Anatomical file info (from dir()). now_func_path - Struct. Functional file info (from dir()). slover_slices - Vector. Indices of slices to display. slover_contour_range - Vector. Range for contour levels (e.g., [0.5 0.5]). slover_view - String. 'axial', 'sagittal', or 'coronal'. ss - Boolean. Space toggle (1 = Subject, 0 = MNI). quality_cont

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `name_` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `ss` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `spm_check_registration_evalc`, `whifun_slover`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `spm_check_registration_evalc`, `whifun_slover`
