# Module Name: `whifun_functions/whifun_normalise_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_NORMALISE_PREPROC Orchestrates normalization to MNI space. [Subj_list_1, out_func_path, out_anat_path] = WHIFUN_NORMALISE_PREPROC(...) is a high-level function that manages the spatial normalization step of a neuroimaging preprocessing pipeline. It applies a previously calculated deformation field (from the segmentation step) to both functional and anatomical images, transforming them from the subject's native space to a standard template space (MNI). The function performs the normalization in two separate steps: 1. **Functional Normalization**: It checks for an existing normalized func
  - Internal calls detected: `reslice_data`, `whifun_anat_mask`, `whifun_create_file`, `whifun_normalise`, `write_error`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_normalise_preproc()`

### Syntax
```matlab
function [Subj_list_1,out_func_path,out_anat_path] = whifun_normalise_preproc(quality_control_path,Subj_list_1,in_func_path,in_anat_path,in_def_path,vox,Norm_pre,GM_path,WM_path,CSF_path,log_fileID,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_NORMALISE_PREPROC Orchestrates normalization to MNI space. [Subj_list_1, out_func_path, out_anat_path] = WHIFUN_NORMALISE_PREPROC(...) is a high-level function that manages the spatial normalization step of a neuroimaging preprocessing pipeline. It applies a previously calculated deformation field (from the segmentation step) to both functional and anatomical images, transforming them from the subject's native space to a standard template space (MNI). The function performs the normalization in two separate steps: 1. **Functional Normalization**: It checks for an existing normalized functional file and, based on the `over_write` flag, either skips or calls `whifun_normalise` to perform

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_def_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vox` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Norm_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `GM_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WM_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `CSF_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `log_fileID` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `out_func_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `out_anat_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `reslice_data`, `whifun_anat_mask`, `whifun_create_file`, `whifun_normalise`, `write_error`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_preproc.m:1/whifun_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `reslice_data`, `whifun_anat_mask`, `whifun_create_file`, `whifun_normalise`, `write_error`
- Related callers: `whifun_functions/whifun_preproc.m:1/whifun_preproc`
