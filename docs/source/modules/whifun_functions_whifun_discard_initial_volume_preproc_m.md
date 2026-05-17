# Module Name: `whifun_functions/whifun_discard_initial_volume_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_DISCARD_INITIAL_VOLUME Removes initial volumes from a functional scan. Subj_list_1 = WHIFUN_DISCARD_INITIAL_VOLUME(quality_control_path, Subj_list_1, ..., over_write) discards a specified number of initial volumes (`n_vol_dis`) from a functional NIfTI file. This is a common step in fMRI preprocessing to allow for signal to stabilize. The function first checks if the output file already exists and, based on the `over_write` flag, either uses the existing file or deletes it and creates a new one. It then reads the functional data, discards the initial volumes, and saves the new file. The
  - Internal calls detected: `niftisave`, `whifun_create_file`, `whifun_multiple_file_found`, `write_error`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_discard_initial_volume_preproc()`

### Syntax
```matlab
function Subj_list_1 = whifun_discard_initial_volume_preproc(quality_control_path,Subj_list_1,in_func_path,out_func_path,n_vol_dis,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_DISCARD_INITIAL_VOLUME Removes initial volumes from a functional scan. Subj_list_1 = WHIFUN_DISCARD_INITIAL_VOLUME(quality_control_path, Subj_list_1, ..., over_write) discards a specified number of initial volumes (`n_vol_dis`) from a functional NIfTI file. This is a common step in fMRI preprocessing to allow for signal to stabilize. The function first checks if the output file already exists and, based on the `over_write` flag, either uses the existing file or deletes it and creates a new one. It then reads the functional data, discards the initial volumes, and saves the new file. The subject structure is updated with the path to the new file and the new number of time points. In cas

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n_vol_dis` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `whifun_create_file`, `whifun_multiple_file_found`, `write_error`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_post_proc_hcp.m:1/whifun_post_proc_hcp`, `whifun_functions/whifun_post_proc_hcp_dev.m:1/whifun_post_proc_hcp_dev`, `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `whifun_create_file`, `whifun_multiple_file_found`, `write_error`
- Related callers: `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_post_proc_hcp.m:1/whifun_post_proc_hcp`, `whifun_functions/whifun_post_proc_hcp_dev.m:1/whifun_post_proc_hcp_dev`, `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`
