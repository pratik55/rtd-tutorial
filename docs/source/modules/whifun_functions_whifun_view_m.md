# Module Name: `whifun_functions/whifun_view.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
  - Internal calls detected: `whifun_convert_coords`
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `whifun_view()`
- **Signature & Definition:** `function whifun_view(vol, M)` (line 1)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transformation matrix (from NIfTI header) for converting Voxel coordinates to MNI/World coordinates. Depen
- **Arguments:**
  - `vol` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `M` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_convert_coords`
  - External: MATLAB NIfTI I/O
  - Called By: `main.mlapp:2534/CheckMaskButtonPushed`, `main.mlapp:2544/CheckMaskButton_2Pushed`, `main.mlapp:2554/CheckatlasButtonPushed`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

## Function: `clickXZ1()`
- **Signature & Definition:** `function clickXZ1(~,evt)` (line 159)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `~` (unused placeholder): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `evt` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `clickYZ()`
- **Signature & Definition:** `function clickYZ(~,evt)` (line 163)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `~` (unused placeholder): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `evt` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `clickXY1()`
- **Signature & Definition:** `function clickXY1(~,evt)` (line 167)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `~` (unused placeholder): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `evt` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `editBoxCallback()`
- **Signature & Definition:** `function editBoxCallback(src,dim,type)` (line 172)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `src` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `dim` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `type` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_convert_coords`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.

## Function: `changeVolume()`
- **Signature & Definition:** `function changeVolume(src)` (line 189)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `src` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

## Function: `sliderVolume()`
- **Signature & Definition:** `function sliderVolume(src)` (line 201)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `src` (MATLAB App/UI object or callback handle): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.

## Function: `updateViews()`
- **Signature & Definition:** `function updateViews(h)` (line 212)
- **Scientific Theory & Formulas:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_VIEW Ortho viewer for 3D or 4D NIfTI volumes with interactive crosshairs, coordinate display (Voxel and optional MNI), volume navigation, and time series plotting. Usage: whifun_view(vol4d, M) % Pass 4D volume data and affine matrix M whifun_view(vol3d) % Pass 3D volume data whifun_view(nifti_path) % Pass NIfTI file path (reads data and header M) Input Arguments: VOL: Input data. Can be: - X x Y x Z x T numeric array (4D fMRI data). - X x Y x Z numeric array (3D anatomical/map data). - Character array or string specifying the path to a NIfTI file. M: (Optional) 4x4 numeric affine transf
- **Arguments:**
  - `h` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_convert_coords`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.
