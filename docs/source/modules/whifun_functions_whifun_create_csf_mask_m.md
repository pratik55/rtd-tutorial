# Module Name: `whifun_functions/whifun_create_csf_mask.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_CSF_MASK Creates a CSF mask using SPM's imcalc. output = WHIFUN_CREATE_CSF_MASK(csf_tpm_path, now_func_path, CSF_thres) generates a binary mask of the Cerebrospinal Fluid (CSF) in the functional image's native space. This mask is based on a CSF tissue probability map (TPM). The function uses SPM's `imcalc` to apply a threshold to the CSF TPM (Output of Segmentation). The functional image is included as a reference to define the output image's dimensions and header information, ensuring the mask is in the correct space. The process involves the following steps: 1. **Input Selectio
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12, Shell/system execution

## `whifun_create_csf_mask()`

### Syntax
```matlab
function output = whifun_create_csf_mask(csf_tpm_path,now_func_path,CSF_thres)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_CSF_MASK Creates a CSF mask using SPM's imcalc. output = WHIFUN_CREATE_CSF_MASK(csf_tpm_path, now_func_path, CSF_thres) generates a binary mask of the Cerebrospinal Fluid (CSF) in the functional image's native space. This mask is based on a CSF tissue probability map (TPM). The function uses SPM's `imcalc` to apply a threshold to the CSF TPM (Output of Segmentation). The functional image is included as a reference to define the output image's dimensions and header information, ensuring the mask is in the correct space. The process involves the following steps: 1. **Input Selection**: The CSF TPM and the first volume of the functional image are provided as inputs to `imcalc`. 2.

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `csf_tpm_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `now_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `CSF_thres` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `output` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** SPM12, Shell/system execution
- **Called By:** `whifun_functions/whifun_csf_mask_extraction_preproc.m:1/whifun_csf_mask_extraction_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `whifun_functions/whifun_csf_mask_extraction_preproc.m:1/whifun_csf_mask_extraction_preproc`
