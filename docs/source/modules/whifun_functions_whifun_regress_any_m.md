# Module Name: `whifun_functions/whifun_regress_any.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_REGRESS_ANY Performs voxel-wise nuisance regression on a 4D NIfTI. FUNC_MASK_PATH = WHIFUN_REGRESS_ANY(IN_FUNC_PATH, IN_ANAT_MASK, ... CONFOUNDS_MATRIX, OUT_FUNC_PATH) reads a functional NIfTI file, removes signals defined in the confounds matrix using linear regression, adds the mean signal back, and saves the result. INPUTS: in_func_path - String. Path to the input 4D functional NIfTI. in_anat_mask - String. Path to the anatomical mask NIfTI. confounds_matrix - Matrix (T x N). Nuisance regressors (e.g., motion parameters, CSF signal) where T matches the number of timepoints. out_func_
  - Internal calls detected: `niftisave`, `whifun_create_rest_mask`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, Statistics and Machine Learning Toolbox

## `whifun_regress_any()`

### Syntax
```matlab
function func_mask_path = whifun_regress_any(in_func_path,in_anat_mask,confounds_matrix,out_func_path)
```
Defined at source line `1`.

### Description
WHIFUN_REGRESS_ANY Performs voxel-wise nuisance regression on a 4D NIfTI. FUNC_MASK_PATH = WHIFUN_REGRESS_ANY(IN_FUNC_PATH, IN_ANAT_MASK, ... CONFOUNDS_MATRIX, OUT_FUNC_PATH) reads a functional NIfTI file, removes signals defined in the confounds matrix using linear regression, adds the mean signal back, and saves the result. INPUTS: in_func_path - String. Path to the input 4D functional NIfTI. in_anat_mask - String. Path to the anatomical mask NIfTI. confounds_matrix - Matrix (T x N). Nuisance regressors (e.g., motion parameters, CSF signal) where T matches the number of timepoints. out_func_path - String. Path where the regressed NIfTI will be saved. OUTPUTS: func_mask_path - String. Path

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_anat_mask` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `confounds_matrix` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `func_mask_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `whifun_create_rest_mask`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, Statistics and Machine Learning Toolbox
- **Called By:** `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `whifun_create_rest_mask`, `whifun_niftiread`
- Related callers: `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`
