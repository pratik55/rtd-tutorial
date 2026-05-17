# Module Name: `whifun_functions/whifun_partial_corr.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$. Partial correlation removes covariates $Z$: $r_{xy\cdot Z}=\frac{r_{xy}-r_{xZ}R_{ZZ}^{-1}r_{Zy}}{\sqrt{(1-r_{xZ}R_{ZZ}^{-1}r_{Zx})(1-r_{yZ}R_{ZZ}^{-1}r_{Zy})}}$. Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_PARTIAL_CORR Computes the partial correlation between the time series of voxels in a target mask and the average time series of a set of functional networks (FNs), controlling for all other FNs. PCOR_TS_PATH = WHIFUN_PARTIAL_CORR(WM_OR_GM, MASK_SUBJ_TS_FOLDER, AVG_TS_PATH, FR_MASK_PATH, SUBJ_LIST, K, OVER_WRITE, D_FLAG, D, STEPS, TOT_STEPS) This function calculates the individual-level partial correlation maps (Fisher-z transformed) between every voxel's time series in the target `fr_mask` and each of the K functional networks (WM-FN or GM-FN), while regressing out the influence of the
  - Internal calls detected: `whifun_create_file`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox, ANTs command-line suite

## `whifun_partial_corr()`

### Syntax
```matlab
function pcor_ts_path = whifun_partial_corr(WM_or_GM,mask_subj_ts_folder,avg_ts_path,fr_mask_path,Subj_list,K,over_write,d_flag,d,steps,tot_steps)
```
Defined at source line `1`.

### Description
WHIFUN_PARTIAL_CORR Computes the partial correlation between the time series of voxels in a target mask and the average time series of a set of functional networks (FNs), controlling for all other FNs. PCOR_TS_PATH = WHIFUN_PARTIAL_CORR(WM_OR_GM, MASK_SUBJ_TS_FOLDER, AVG_TS_PATH, FR_MASK_PATH, SUBJ_LIST, K, OVER_WRITE, D_FLAG, D, STEPS, TOT_STEPS) This function calculates the individual-level partial correlation maps (Fisher-z transformed) between every voxel's time series in the target `fr_mask` and each of the K functional networks (WM-FN or GM-FN), while regressing out the influence of the other K-1 networks. Input Arguments: WM_OR_GM - String indicating the network type (e.g., 'WM' or 'G

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `WM_or_GM` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `mask_subj_ts_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `avg_ts_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `fr_mask_path` — character vector or string scalar filesystem path
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

#### `steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tot_steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `pcor_ts_path` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$. Partial correlation removes covariates $Z$: $r_{xy\cdot Z}=\frac{r_{xy}-r_{xZ}R_{ZZ}^{-1}r_{Zy}}{\sqrt{(1-r_{xZ}R_{ZZ}^{-1}r_{Zx})(1-r_{yZ}R_{ZZ}^{-1}r_{Zy})}}$. Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. Fisher transformation uses $z=\operatorname{atanh}(r)=\frac{1}{2}\ln\frac{1+r}{1-r}$. Partial correlation removes covariates $Z$: $r_{xy\cdot Z}=\frac{r_{xy}-r_{xZ}R_{ZZ}^{-1}r_{Zy}}{\sqrt{(1-r_{xZ}R_{ZZ}^{-1}r_{Zx})(1-r_{yZ}R_{ZZ}^{-1}r_{Zy})}}$. Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox, ANTs command-line suite
- **Called By:** `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`
- Related callers: `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`
