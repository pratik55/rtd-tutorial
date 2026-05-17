# Module Name: `whifun_functions/whifun_nuisance_regress_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_NUISANCE_REGRESS_PREPROC Orchestrates nuisance regression. [Subj_list_1, out_func_path] = WHIFUN_NUISANCE_REGRESS_PREPROC(...) is a high-level function that manages the nuisance regression step of a neuroimaging preprocessing pipeline. It automates the process of removing unwanted signals from the functional data, such as head motion artifacts and physiological noise. The function first checks if a pre-regressed file already exists. Based on the `over_write` flag, it either skips the process or calls the `whifun_regress` function to perform the actual regression. This utility function e
  - Internal calls detected: `whifun_create_file`, `whifun_regress`, `write_error`
  - External dependencies detected: Shell/system execution

## `whifun_nuisance_regress_preproc()`

### Syntax
```matlab
function [Subj_list_1,out_func_path,out_func_mask_path] = whifun_nuisance_regress_preproc(quality_control_path,Subj_list_1,in_func_path,in_anat_mask_subj_space_path,Reg_pre,n_pca,in_csf_mat_path,in_motion_txt_path,log_fileID,over_write) %#ok<INUSD>
```
Defined at source line `1`.

### Description
WHIFUN_NUISANCE_REGRESS_PREPROC Orchestrates nuisance regression. [Subj_list_1, out_func_path] = WHIFUN_NUISANCE_REGRESS_PREPROC(...) is a high-level function that manages the nuisance regression step of a neuroimaging preprocessing pipeline. It automates the process of removing unwanted signals from the functional data, such as head motion artifacts and physiological noise. The function first checks if a pre-regressed file already exists. Based on the `over_write` flag, it either skips the process or calls the `whifun_regress` function to perform the actual regression. This utility function ensures that the regression is performed only when needed. The function updates the subject structure

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
- No explicit input arguments.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

#### `out_func_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

#### `out_func_mask_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_regress`, `write_error`
- **External Dependencies:** Shell/system execution
- **Called By:** `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_regress`, `write_error`
- Related callers: `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`
