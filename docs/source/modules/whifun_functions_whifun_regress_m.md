# Module Name: `whifun_functions/whifun_regress.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_REGRESS Performs nuisance regression on functional data. func_mask_path = WHIFUN_REGRESS(in_func_path, ..., n_pca) performs nuisance regression on a functional neuroimaging time series. This process removes signals from non-neuronal sources, such as head motion and physiological noise. The function first loads the functional data and creates a brain mask by reslicing an anatomical mask into functional space. It then constructs a design matrix (`b_init`) of nuisance regressors, which can include: - **CSF Signal**: Loaded from `in_csf_mat_path`. The signal can be either the mean CSF time
  - Internal calls detected: `niftisave`, `whifun_create_rest_mask`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox

## `whifun_regress()`

### Syntax
```matlab
function func_mask_path = whifun_regress(in_func_path,in_anat_mask_subj_space_path,in_csf_mat_path,in_motion_txt_path,out_func_path,n_pca)
```
Defined at source line `1`.

### Description
WHIFUN_REGRESS Performs nuisance regression on functional data. func_mask_path = WHIFUN_REGRESS(in_func_path, ..., n_pca) performs nuisance regression on a functional neuroimaging time series. This process removes signals from non-neuronal sources, such as head motion and physiological noise. The function first loads the functional data and creates a brain mask by reslicing an anatomical mask into functional space. It then constructs a design matrix (`b_init`) of nuisance regressors, which can include: - **CSF Signal**: Loaded from `in_csf_mat_path`. The signal can be either the mean CSF time series or a set of PCA components. - **Motion Parameters**: Loaded from `in_motion_txt_path`. If `mo

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `in_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_anat_mask_subj_space_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_csf_mat_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `in_motion_txt_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `out_func_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `n_pca` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `func_mask_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `whifun_create_rest_mask`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox
- **Called By:** `whifun_functions/whifun_nuisance_regress_preproc.m:1/whifun_nuisance_regress_preproc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `whifun_create_rest_mask`, `whifun_niftiread`
- Related callers: `whifun_functions/whifun_nuisance_regress_preproc.m:1/whifun_nuisance_regress_preproc`
