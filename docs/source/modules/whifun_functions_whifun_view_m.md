# Module Name: `whifun_functions/whifun_view.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
  - Internal calls detected: `whifun_convert_coords`
  - External dependencies detected: MATLAB NIfTI I/O

## `whifun_view()`

### Syntax
```matlab
function whifun_view(vol, M)
```
Defined at source line `1`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transformation matrix (from NIfTI header) for converting Voxel coordinates to MNI/World coordinates. Depen

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `vol` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `M` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_convert_coords`
- **External Dependencies:** MATLAB NIfTI I/O
- **Called By:** `main.mlapp:2534/CheckMaskButtonPushed`, `main.mlapp:2544/CheckMaskButton_2Pushed`, `main.mlapp:2554/CheckatlasButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_convert_coords`
- Related callers: `main.mlapp:2534/CheckMaskButtonPushed`, `main.mlapp:2544/CheckMaskButton_2Pushed`, `main.mlapp:2554/CheckatlasButtonPushed`

## `clickXZ1()`

### Syntax
```matlab
function clickXZ1(~,evt)
```
Defined at source line `159`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `evt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `clickYZ()`

### Syntax
```matlab
function clickYZ(~,evt)
```
Defined at source line `163`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `evt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `clickXY1()`

### Syntax
```matlab
function clickXY1(~,evt)
```
Defined at source line `167`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `~` — unused placeholder
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `evt` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `editBoxCallback()`

### Syntax
```matlab
function editBoxCallback(src,dim,type)
```
Defined at source line `172`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `src` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `dim` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `type` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_convert_coords`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_convert_coords`

## `changeVolume()`

### Syntax
```matlab
function changeVolume(src)
```
Defined at source line `189`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `src` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `sliderVolume()`

### Syntax
```matlab
function sliderVolume(src)
```
Defined at source line `201`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `src` — MATLAB App/UI object or callback handle
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.

## `updateViews()`

### Syntax
```matlab
function updateViews(h)
```
Defined at source line `212`.

### Description
WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `h` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_convert_coords`
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_convert_coords`
