# Module Name: `whifun_functions/whifun_coreg_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COREG_PREPROC Orchestrates SPM-based anatomical-functional coregistration. Subj_list_1 = WHIFUN_COREG_PREPROC(quality_control_path, ..., over_write) is a high-level function that manages the coregistration step of a neuroimaging preprocessing pipeline. Coregistration is the process of aligning a subject's functional scans to their high-resolution anatomical scan. The function first checks if a coregistration has already been performed by comparing the transformation matrices of the input and image before realigned functional files. If they are different or `over_write` is enabled, it pr
  - Internal calls detected: `whifun_coreg`, `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_coreg_preproc()`

### Syntax
```matlab
function Subj_list_1  = whifun_coreg_preproc(quality_control_path,Subj_list_1,in_func_path_bef,in_func_path_after,in_anat_path,log_fileID,over_write,no_mean_func)
```
Defined at source line `1`.

### Description
WHIFUN_COREG_PREPROC Orchestrates SPM-based anatomical-functional coregistration. Subj_list_1 = WHIFUN_COREG_PREPROC(quality_control_path, ..., over_write) is a high-level function that manages the coregistration step of a neuroimaging preprocessing pipeline. Coregistration is the process of aligning a subject's functional scans to their high-resolution anatomical scan. The function first checks if a coregistration has already been performed by comparing the transformation matrices of the input and image before realigned functional files. If they are different or `over_write` is enabled, it proceeds. The function then calls `whifun_coreg` to perform the actual SPM coregistration job. The new

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path_bef` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path_after` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_anat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `log_fileID` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `no_mean_func` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_coreg`, `write_error`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_preproc.m:1/whifun_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_coreg`, `write_error`
- Related callers: `whifun_functions/whifun_preproc.m:1/whifun_preproc`
