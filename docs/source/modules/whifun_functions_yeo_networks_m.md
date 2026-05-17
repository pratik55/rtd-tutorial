# Module Name: `whifun_functions/yeo_networks.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - % Networks of Yeo Written by Pratik Jain Maps every ROI of the given atlas to one of the 7 Resting state networks of yeo Input --> atlas_brain (Data type = Char) = Path of the brain atlas (nifti file) whose ROIs are to be mapped atlas_yeo (Data type = Char) = Path of the yeo brain atlas (nifti file) Output --> idx = vector numbering every ROI to a yeo 7 network if idx(i) = 1 --> ith node belongs to Visual network if idx(i) = 2 --> ith node belongs to Somatomotor network if idx(i) = 3 --> ith node belongs to Dorsal Attention network if idx(i) = 4 --> ith node belongs to Ventral Attention networ
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O

## `yeo_networks()`

### Syntax
```matlab
function idx = yeo_networks(atlas_brain_path,atlas_yeo_path)
```
Defined at source line `1`.

### Description
% Networks of Yeo Written by Pratik Jain Maps every ROI of the given atlas to one of the 7 Resting state networks of yeo Input --> atlas_brain (Data type = Char) = Path of the brain atlas (nifti file) whose ROIs are to be mapped atlas_yeo (Data type = Char) = Path of the yeo brain atlas (nifti file) Output --> idx = vector numbering every ROI to a yeo 7 network if idx(i) = 1 --> ith node belongs to Visual network if idx(i) = 2 --> ith node belongs to Somatomotor network if idx(i) = 3 --> ith node belongs to Dorsal Attention network if idx(i) = 4 --> ith node belongs to Ventral Attention network if idx(i) = 5 --> ith node belongs to Limbic network if idx(i) = 6 --> ith node belongs to Fronto-

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `atlas_brain_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `atlas_yeo_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `idx` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.
