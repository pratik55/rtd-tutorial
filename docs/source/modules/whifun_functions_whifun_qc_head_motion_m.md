# Module Name: `whifun_functions/whifun_qc_head_motion.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_HEAD_MOTION Generates a quality control figure for head motion. WHIFUN_QC_HEAD_MOTION(out_folder, realigned_func_native, ..., motion_txt) creates a comprehensive quality control report for head motion for a single subject. The report consists of four plots combined into a single figure. The function performs the following steps: 1. **Check Existence**: It checks if a head motion QC image already exists and, based on the `over_write` flag, either skips or generates a new one. 2. **Calculate Metrics**: It reads the realigned functional data and the motion parameter file. It then calcul
  - Internal calls detected: `whifun_create_file`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O

## `whifun_qc_head_motion()`

### Syntax
```matlab
function whifun_qc_head_motion(out_folder,realigned_func_native,name,max_fd,mean_fd,greater_than_20,over_write,motion_txt)
```
Defined at source line `1`.

### Description
WHIFUN_QC_HEAD_MOTION Generates a quality control figure for head motion. WHIFUN_QC_HEAD_MOTION(out_folder, realigned_func_native, ..., motion_txt) creates a comprehensive quality control report for head motion for a single subject. The report consists of four plots combined into a single figure. The function performs the following steps: 1. **Check Existence**: It checks if a head motion QC image already exists and, based on the `over_write` flag, either skips or generates a new one. 2. **Calculate Metrics**: It reads the realigned functional data and the motion parameter file. It then calculates: - **Global Mean**: The scaled global signal mean over time. - **Pairwise Variance**: A measure

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `realigned_func_native` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `max_fd` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mean_fd` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `greater_than_20` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `motion_txt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`
