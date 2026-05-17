# Module Name: `whifun_functions/whifun_show_slices_multioverlay.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_SHOW_SLICES_MULTIOVERLAY Display multiple slices (one per image) in a montage with overlay support. Inputs: volumes - cell array of file paths or 3D matrices overlay_types - cell array: {'structure','contour',...} cmaps - cell array of colormaps for each image slices - array of slice indices (one per image) orientation - 'axial' | 'sagittal' | 'coronal' Example: vols = {'sub1.nii','sub2.nii','sub3.nii'}; types = {'structure','contour','structure'}; cmaps = {hot, lines, gray}; slices = [40 45 50]; whifun_show_slices_multioverlay(vols, types, cmaps, slices, 'axial'); --- Input checks ---
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O, Image Processing Toolbox

## `whifun_show_slices_multioverlay()`

### Syntax
```matlab
function whifun_show_slices_multioverlay(volumes, overlay_types, cmaps, slices, orientation)
```
Defined at source line `1`.

### Description
WHIFUN_SHOW_SLICES_MULTIOVERLAY Display multiple slices (one per image) in a montage with overlay support. Inputs: volumes - cell array of file paths or 3D matrices overlay_types - cell array: {'structure','contour',...} cmaps - cell array of colormaps for each image slices - array of slice indices (one per image) orientation - 'axial' | 'sagittal' | 'coronal' Example: vols = {'sub1.nii','sub2.nii','sub3.nii'}; types = {'structure','contour','structure'}; cmaps = {hot, lines, gray}; slices = [40 45 50]; whifun_show_slices_multioverlay(vols, types, cmaps, slices, 'axial'); --- Input checks ---

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `volumes` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `overlay_types` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `cmaps` — numeric scalar, vector, matrix, or multidimensional array
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slices` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `orientation` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** MATLAB NIfTI I/O, Image Processing Toolbox
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `capitalize()`

### Syntax
```matlab
function s = capitalize(str)
```
Defined at source line `88`.

### Description
WHIFUN_SHOW_SLICES_MULTIOVERLAY Display multiple slices (one per image) in a montage with overlay support. Inputs: volumes - cell array of file paths or 3D matrices overlay_types - cell array: {'structure','contour',...} cmaps - cell array of colormaps for each image slices - array of slice indices (one per image) orientation - 'axial' | 'sagittal' | 'coronal' Example: vols = {'sub1.nii','sub2.nii','sub3.nii'}; types = {'structure','contour','structure'}; cmaps = {hot, lines, gray}; slices = [40 45 50]; whifun_show_slices_multioverlay(vols, types, cmaps, slices, 'axial'); --- Input checks ---

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `str` — numeric scalar or numeric vector
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `s` — numeric scalar or numeric vector
Output produced by the MATLAB implementation.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.
