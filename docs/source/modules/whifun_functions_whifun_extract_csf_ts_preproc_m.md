# Module Name: `whifun_functions/whifun_extract_csf_ts_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_EXTRACT_CSF_TS_PREPROC Extracts and preprocesses CSF time series data. [Subj_list_1, out_csf_mat_path] = WHIFUN_EXTRACT_CSF_TS_PREPROC(...) is a high-level function that manages the extraction of the Cerebrospinal Fluid (CSF) signal from a functional scan. This time series is often used as a nuisance regressor to reduce non-neuronal signal in fMRI data. The function first checks if a pre-existing CSF time series file (e.g., `.mat` file) exists. Based on the `over_write` flag, it either skips the process or calls the `whifun_extract_csf_ts` function to perform the extraction. The functio
  - Internal calls detected: `whifun_create_file`, `whifun_extract_csf_ts`, `write_error`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_extract_csf_ts_preproc()`

### Syntax
```matlab
function [Subj_list_1,out_csf_mat_path] = whifun_extract_csf_ts_preproc(quality_control_path,Subj_list_1,in_func_path,in_csf_mask_func_path,pca_for_temp_reg,n_pca,log_fileID,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_EXTRACT_CSF_TS_PREPROC Extracts and preprocesses CSF time series data. [Subj_list_1, out_csf_mat_path] = WHIFUN_EXTRACT_CSF_TS_PREPROC(...) is a high-level function that manages the extraction of the Cerebrospinal Fluid (CSF) signal from a functional scan. This time series is often used as a nuisance regressor to reduce non-neuronal signal in fMRI data. The function first checks if a pre-existing CSF time series file (e.g., `.mat` file) exists. Based on the `over_write` flag, it either skips the process or calls the `whifun_extract_csf_ts` function to perform the extraction. The function handles the option of performing Principal Component Analysis (PCA) on the extracted time series.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_csf_mask_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `pca_for_temp_reg` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n_pca` — numeric scalar or numeric vector
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

#### `out_csf_mat_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_extract_csf_ts`, `write_error`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_extract_csf_ts`, `write_error`
- Related callers: `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`
