# Module Name: `whifun_functions/whifun_create_brainnet_images.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_CREATE_BRAINNET_IMAGES Generates a series of PNG images for each network in a labeled NIfTI volume using the BrainNet Viewer toolbox. WHIFUN_CREATE_BRAINNET_IMAGES(OUT_PATH, ROI_PATH, OVER_WRITE) This function iterates through all unique network labels in the input ROI NIfTI file and creates a visualization of each network from multiple standard viewing angles using BrainNet Viewer. Input Arguments: OUT_PATH - The directory where the resulting PNG images will be saved. ROI_PATH - The full path to the input NIfTI file containing the labeled Functional Network (FN) map (e.g., 'WM_clusteri
  - Internal calls detected: `BrainNet_MapCfg_WhifuN`, `whifun_create_file`, `whifun_niftiread`
  - External dependencies detected: MATLAB NIfTI I/O, BrainNet Viewer

## `whifun_create_brainnet_images()`

### Syntax
```matlab
function whifun_create_brainnet_images(out_path,ROI_path,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_CREATE_BRAINNET_IMAGES Generates a series of PNG images for each network in a labeled NIfTI volume using the BrainNet Viewer toolbox. WHIFUN_CREATE_BRAINNET_IMAGES(OUT_PATH, ROI_PATH, OVER_WRITE) This function iterates through all unique network labels in the input ROI NIfTI file and creates a visualization of each network from multiple standard viewing angles using BrainNet Viewer. Input Arguments: OUT_PATH - The directory where the resulting PNG images will be saved. ROI_PATH - The full path to the input NIfTI file containing the labeled Functional Network (FN) map (e.g., 'WM_clustering_K10.nii'). OVER_WRITE - Flag (0 or 1). If 0, image generation will be skipped if the first output

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `ROI_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.

### Algorithms
K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `BrainNet_MapCfg_WhifuN`, `whifun_create_file`, `whifun_niftiread`
- **External Dependencies:** MATLAB NIfTI I/O, BrainNet Viewer
- **Called By:** `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `BrainNet_MapCfg_WhifuN`, `whifun_create_file`, `whifun_niftiread`
- Related callers: `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`
