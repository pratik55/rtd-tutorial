# Module Name: `whifun_functions/whifun_create_fn_from_parrcorr_and_ttest.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Partial correlation removes covariates $Z$: $r_{xy\cdot Z}=\frac{r_{xy}-r_{xZ}R_{ZZ}^{-1}r_{Zy}}{\sqrt{(1-r_{xZ}R_{ZZ}^{-1}r_{Zx})(1-r_{yZ}R_{ZZ}^{-1}r_{Zy})}}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_FN_FROM_PARRCORR_AND_TTEST Creates a new Functional Network (FN) map by assigning each voxel in a target mask (e.g., Corpus Callosum) to the existing network (e.g., WM or GM) with which it shares the maximal significant partial correlation. FN_PATH = WHIFUN_CREATE_FN_FROM_PARRCORR_AND_TTEST(WM_OR_GM, PCOR_TS_PATH, MASK_PATH, SUBJ_LIST, K, OVER_WRITE, ...) This is used to extend existing FN definitions (like WM-FNs) into other regions (like the Corpus Callosum or Cerebellum) based on connectivity. The assignment metric is the group-level t-statistic of the partial correlation acro
  - Internal calls detected: `niftisave`, `whifun_create_file`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox

## `whifun_create_fn_from_parrcorr_and_ttest()`

### Syntax
```matlab
function fn_path = whifun_create_fn_from_parrcorr_and_ttest(WM_or_GM,pcor_ts_path,mask_path,Subj_list,K,over_write,d_flag,d,wm_steps,tot_wm_steps)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_FN_FROM_PARRCORR_AND_TTEST Creates a new Functional Network (FN) map by assigning each voxel in a target mask (e.g., Corpus Callosum) to the existing network (e.g., WM or GM) with which it shares the maximal significant partial correlation. FN_PATH = WHIFUN_CREATE_FN_FROM_PARRCORR_AND_TTEST(WM_OR_GM, PCOR_TS_PATH, MASK_PATH, SUBJ_LIST, K, OVER_WRITE, ...) This is used to extend existing FN definitions (like WM-FNs) into other regions (like the Corpus Callosum or Cerebellum) based on connectivity. The assignment metric is the group-level t-statistic of the partial correlation across subjects. Input Arguments: WM_OR_GM - String ('WM' or 'GM') indicating the type of network used a

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `WM_or_GM` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `pcor_ts_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mask_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `K` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d_flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `wm_steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tot_wm_steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `fn_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Partial correlation removes covariates $Z$: $r_{xy\cdot Z}=\frac{r_{xy}-r_{xZ}R_{ZZ}^{-1}r_{Zy}}{\sqrt{(1-r_{xZ}R_{ZZ}^{-1}r_{Zx})(1-r_{yZ}R_{ZZ}^{-1}r_{Zy})}}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Partial correlation removes covariates $Z$: $r_{xy\cdot Z}=\frac{r_{xy}-r_{xZ}R_{ZZ}^{-1}r_{Zy}}{\sqrt{(1-r_{xZ}R_{ZZ}^{-1}r_{Zx})(1-r_{yZ}R_{ZZ}^{-1}r_{Zy})}}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `whifun_create_file`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox
- **Called By:** `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `whifun_create_file`, `whifun_niftiread`
- Related callers: `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`
