# Module Name: `whifun_functions/whifun_csf_mask_extraction_preproc.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CSF_MASK_EXTRACTION_PREPROC Creates a CSF mask in functional space. [Subj_list_1, out_csf_mask_func_path] = WHIFUN_CSF_MASK_EXTRACTION_PREPROC(...) is a high-level function that manages the creation of a Cerebrospinal Fluid (CSF) mask in the functional image's native space. This mask is often used to extract a mean CSF signal for nuisance regression. The function first checks for the input functional file and the CSF tissue probability map (TPM). It then determines the output file path for the CSF mask and, based on the `over_write` flag, either skips the process or proceeds by calling
  - Internal calls detected: `whifun_create_csf_mask`, `whifun_create_file`, `write_error`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_csf_mask_extraction_preproc()`

### Syntax
```matlab
function [Subj_list_1,out_csf_mask_func_path] = whifun_csf_mask_extraction_preproc(quality_control_path,Subj_list_1,in_func_path,in_csf_tpm_path,CSF_thres,log_fileID,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_CSF_MASK_EXTRACTION_PREPROC Creates a CSF mask in functional space. [Subj_list_1, out_csf_mask_func_path] = WHIFUN_CSF_MASK_EXTRACTION_PREPROC(...) is a high-level function that manages the creation of a Cerebrospinal Fluid (CSF) mask in the functional image's native space. This mask is often used to extract a mean CSF signal for nuisance regression. The function first checks for the input functional file and the CSF tissue probability map (TPM). It then determines the output file path for the CSF mask and, based on the `over_write` flag, either skips the process or proceeds by calling `whifun_create_csf_mask`. The function updates the subject structure with the path to the newly crea

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_csf_tpm_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `CSF_thres` — numeric scalar or numeric vector
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

#### `out_csf_mask_func_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_csf_mask`, `whifun_create_file`, `write_error`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_csf_mask`, `whifun_create_file`, `write_error`
- Related callers: `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`
