# Module Name: `whifun_functions/whifun_erode.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_ERODE Erodes a binary mask. out_mask_path = WHIFUN_ERODE(path_, num_erosions, out_pre) performs morphological erosion on a binary or probabilistic mask image. Erosion removes voxels from the boundary of a mask, making it smaller. This is often used to create a more central "deep" mask of a tissue type, for example, a deep white matter mask to avoid contamination from gray matter. The function performs the following steps: 1. **Read Image**: It reads the input NIfTI mask file. 2. **Erode**: It iteratively applies SPM's `spm_erode` function a specified number of times (`num_erosions`). 3.
  - Internal calls detected: `niftisave`
  - External dependencies detected: MATLAB NIfTI I/O, SPM12

## `whifun_erode()`

### Syntax
```matlab
function out_mask_path = whifun_erode(path_,num_erosions,out_pre)
```
Defined at source line `1`.

### Description
WHIFUN_ERODE Erodes a binary mask. out_mask_path = WHIFUN_ERODE(path_, num_erosions, out_pre) performs morphological erosion on a binary or probabilistic mask image. Erosion removes voxels from the boundary of a mask, making it smaller. This is often used to create a more central "deep" mask of a tissue type, for example, a deep white matter mask to avoid contamination from gray matter. The function performs the following steps: 1. **Read Image**: It reads the input NIfTI mask file. 2. **Erode**: It iteratively applies SPM's `spm_erode` function a specified number of times (`num_erosions`). 3. **Save Output**: The eroded mask is saved as a new NIfTI file with a name that includes the number

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `path_` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `num_erosions` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_pre` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out_mask_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`
- **External Dependencies:** MATLAB NIfTI I/O, SPM12
- **Called By:** `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`
- Related callers: `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`
