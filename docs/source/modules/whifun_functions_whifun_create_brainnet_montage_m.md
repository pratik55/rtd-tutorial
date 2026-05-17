# Module Name: `whifun_functions/whifun_create_brainnet_montage.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - inputFolder : folder containing WM and GM images outputPrefix: prefix for output files (e.g., 'Networks') Will create 'Networks_WM_montage.png' and 'Networks_GM_montage.png' Define tissue types and views tissueTypes = {'WM', 'GM'};
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: BrainNet Viewer

## `whifun_create_brainnet_montage()`

### Syntax
```matlab
function whifun_create_brainnet_montage(inputFolder, outputPrefix,tissueTypes)
```
Defined at source line `1`.

### Description
inputFolder : folder containing WM and GM images outputPrefix: prefix for output files (e.g., 'Networks') Will create 'Networks_WM_montage.png' and 'Networks_GM_montage.png' Define tissue types and views tissueTypes = {'WM', 'GM'};

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `inputFolder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `outputPrefix` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `tissueTypes` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** BrainNet Viewer
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.
