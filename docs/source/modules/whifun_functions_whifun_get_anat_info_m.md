# Module Name: `whifun_functions/whifun_get_anat_info.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_ANAT_INFO Extracts information from an anatomical NIfTI file. [Subj_list_1, voxel_anat] = WHIFUN_GET_ANAT_INFO(now_anat_path, Subj_list_1) reads metadata from an anatomical neuroimaging NIfTI file specified by `now_anat_path`. The function updates a subject structure with the extracted information and returns the voxel dimensions. This function is a core part of a neuroimaging pipeline, as it retrieves critical anatomical parameters (like voxel size) that are essential for subsequent preprocessing steps such as coregistration and normalization. It handles cases where metadata might
  - Internal calls detected: `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_get_anat_info()`

### Syntax
```matlab
function [Subj_list_1,voxel_anat] = whifun_get_anat_info(now_anat_path,Subj_list_1,output_folder)
```
Defined at source line `1`.

### Description
WHIFUN_GET_ANAT_INFO Extracts information from an anatomical NIfTI file. [Subj_list_1, voxel_anat] = WHIFUN_GET_ANAT_INFO(now_anat_path, Subj_list_1) reads metadata from an anatomical neuroimaging NIfTI file specified by `now_anat_path`. The function updates a subject structure with the extracted information and returns the voxel dimensions. This function is a core part of a neuroimaging pipeline, as it retrieves critical anatomical parameters (like voxel size) that are essential for subsequent preprocessing steps such as coregistration and normalization. It handles cases where metadata might be corrupted or missing. Input Arguments: now_anat_path - A `dir` structure (from a call to `dir`) p

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `now_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `output_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `voxel_anat` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `write_error`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_check_data_anat.m:1/whifun_check_data_anat`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `write_error`
- Related callers: `whifun_functions/whifun_check_data_anat.m:1/whifun_check_data_anat`
