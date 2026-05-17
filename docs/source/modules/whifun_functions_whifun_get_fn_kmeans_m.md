# Module Name: `whifun_functions/whifun_get_FN_kmeans.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_GET_FN_KMEANS Performs k-means clustering on the Voxel-Level Functional Connectivity (FC) matrix to create a Functional Network (FN) map. WHIFUN_GET_FN_KMEANS(OUT_PATH, K, AVG_VOX_LEVEL_FC, WMMASK_, HEADER_FILE, OVER_WRITE, ...) This function takes a group-average FC matrix (where rows are voxels and columns are features) and clusters the voxels into K networks based on the correlation distance metric. The result is saved as a NIfTI volume. Input Arguments: OUT_PATH - Full path to save the resulting FN NIfTI file (e.g., '.../WM_FN_K10.nii'). K - The number of clusters (networks) to crea
  - Internal calls detected: `niftisave`, `whifun_create_file`
  - External dependencies detected: MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox

## `whifun_get_FN_kmeans()`

### Syntax
```matlab
function whifun_get_FN_kmeans(out_path,K,avg_vox_level_FC,WMmask_,header_file,num_replicates,over_write,d_flag,d,steps_,tot_steps)
```
Defined at source line `1`.

### Description
WHIFUN_GET_FN_KMEANS Performs k-means clustering on the Voxel-Level Functional Connectivity (FC) matrix to create a Functional Network (FN) map. WHIFUN_GET_FN_KMEANS(OUT_PATH, K, AVG_VOX_LEVEL_FC, WMMASK_, HEADER_FILE, OVER_WRITE, ...) This function takes a group-average FC matrix (where rows are voxels and columns are features) and clusters the voxels into K networks based on the correlation distance metric. The result is saved as a NIfTI volume. Input Arguments: OUT_PATH - Full path to save the resulting FN NIfTI file (e.g., '.../WM_FN_K10.nii'). K - The number of clusters (networks) to create. Can be a scalar or a vector (though the provided loop suggests it only handles one K at a time).

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `K` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `avg_vox_level_FC` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `WMmask_` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `header_file` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `num_replicates` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d_flag` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `d` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `steps_` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tot_steps` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Pearson FC is $r_{ij}=\frac{\sum_t (x_i(t)-\bar{x}_i)(x_j(t)-\bar{x}_j)}{\sqrt{\sum_t (x_i(t)-\bar{x}_i)^2}\sqrt{\sum_t (x_j(t)-\bar{x}_j)^2}}$; upper-triangle vectorization has length $R(R-1)/2$. K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `niftisave`, `whifun_create_file`
- **External Dependencies:** MATLAB NIfTI I/O, MATLAB table/file I/O, Statistics and Machine Learning Toolbox
- **Called By:** `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `niftisave`, `whifun_create_file`
- Related callers: `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`
