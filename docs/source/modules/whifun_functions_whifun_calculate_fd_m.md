# Module Name: `whifun_functions/whifun_calculate_fd.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CALCULATE_FD Calculates framewise displacement (FD). fd = WHIFUN_CALCULATE_FD(motion) computes the framewise displacement (FD) from motion parameters. FD is a measure of head motion between consecutive time points in an fMRI scan. This function takes either the path to a motion parameter text file (as a string or `dir` structure) or the motion parameters directly (as a numeric matrix). It then calculates the vector difference between each time point. The rotational parameters are converted to millimeters by assuming a brain radius of 50mm, and the absolute sum of all six derivative para
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O

## `whifun_calculate_fd()`

### Syntax
```matlab
function fd = whifun_calculate_fd(motion)
```
Defined at source line `1`.

### Description
WHIFUN_CALCULATE_FD Calculates framewise displacement (FD). fd = WHIFUN_CALCULATE_FD(motion) computes the framewise displacement (FD) from motion parameters. FD is a measure of head motion between consecutive time points in an fMRI scan. This function takes either the path to a motion parameter text file (as a string or `dir` structure) or the motion parameters directly (as a numeric matrix). It then calculates the vector difference between each time point. The rotational parameters are converted to millimeters by assuming a brain radius of 50mm, and the absolute sum of all six derivative parameters is returned as the FD time series. This function is a core part of quality control for fMRI d

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `motion` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `fd` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB table/file I/O
- **Called By:** `whifun_functions/whifun_fd_preproc.m:1/whifun_fd_preproc`, `whifun_functions/whifun_ts_check.m:1/whifun_ts_check`, `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_fd_preproc.m:1/whifun_fd_preproc`, `whifun_functions/whifun_ts_check.m:1/whifun_ts_check`, `whifun_functions/whifun_ts_qc.m:1/whifun_ts_qc`
