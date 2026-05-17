# Module Name: `whifun_functions/Idiff_fun.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - figure;imagesc(A);colorbar;axis image
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## `Idiff_fun()`

### Syntax
```matlab
function out = Idiff_fun(sub_spec,ses)
```
Defined at source line `1`.

### Description
figure;imagesc(A);colorbar;axis image

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `sub_spec` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `ses` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `out` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Identifiability uses $I_{diff}=100(\overline{|r_{self}|}-\overline{|r_{other}|})$ and nearest-neighbor FC matching accuracy. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** Statistics and Machine Learning Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.
