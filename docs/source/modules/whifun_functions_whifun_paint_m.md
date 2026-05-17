# Module Name: `whifun_functions/whifun_paint.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - Method to display slice overlay FORMAT obj = paint(obj, params) Inputs obj - slice overlay object params - optional structure containing extra display parameters - refreshf - overrides refreshf in object - clf - overrides clf in object - userdata - if 0, does not add object to userdata field (see below) Outputs obj - which may have been filled with defaults paint attaches the object used for painting to the 'UserData' field of the figure handle, unless instructed not to with 0 in userdata flag __________________________________________________________________________ Matthew Brett $Id: paint.m
  - Internal calls detected: `findobj`, `mars_struct`, `pr_scaletocmap`
  - External dependencies detected: SPM12, SLover/MarsBaR-style visualization helpers

## `whifun_paint()`

### Syntax
```matlab
function obj = whifun_paint(obj, params)
```
Defined at source line `1`.

### Description
Method to display slice overlay FORMAT obj = paint(obj, params) Inputs obj - slice overlay object params - optional structure containing extra display parameters - refreshf - overrides refreshf in object - clf - overrides clf in object - userdata - if 0, does not add object to userdata field (see below) Outputs obj - which may have been filled with defaults paint attaches the object used for painting to the 'UserData' field of the figure handle, unless instructed not to with 0 in userdata flag __________________________________________________________________________ Matthew Brett $Id: paint.m 6623 2015-12-03 18:38:08Z guillaume $

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `obj` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `params` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `obj` — MATLAB App/UI object or callback handle
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** `findobj`, `mars_struct`, `pr_scaletocmap`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_slover.m:1/whifun_slover`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `findobj`, `mars_struct`, `pr_scaletocmap`
- Related callers: `whifun_functions/whifun_slover.m:1/whifun_slover`

## `sf_slice2panel()`

### Syntax
```matlab
function i1 = sf_slice2panel(img, xyzmm, transform, vdims)
```
Defined at source line `361`.

### Description
to voxel space of image

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `img` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `xyzmm` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `transform` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `vdims` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `i1` — MATLAB value inferred from source usage
Output produced by the MATLAB implementation.

### More About
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.

### Extended Capabilities
- **Internal Calls:** `mars_struct`
- **External Dependencies:** SPM12, SLover/MarsBaR-style visualization helpers
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `mars_struct`
