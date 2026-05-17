# Module Name: `whifun_functions/whifun_multiOverlay.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - whifun_multiOverlay Display multiple slices with overlays from volumes Inputs: volumes - 3D matrix or cell array of volumes (or file paths) overlayTypes - cell array: {'structure','contours'} for each volume colormaps - cell array of colormaps (e.g., {'gray','jet'}) slices - vector of slice indices (e.g. [20 30 40]) sliceType - 'axial','coronal','sagittal' Example: vol1 = rand(50,50,50); vol2 = rand(50,50,50) > 0.7; whifun_multiOverlay({vol1,vol2},{'structure','contours'},{'gray','jet'},[10 20 30],'axial'); % --- Load Volumes ---
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `whifun_multiOverlay()`
- **Signature & Definition:** `function whifun_multiOverlay(volumes, overlayTypes, colormaps, slices, sliceType)` (line 1)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** whifun_multiOverlay Display multiple slices with overlays from volumes Inputs: volumes - 3D matrix or cell array of volumes (or file paths) overlayTypes - cell array: {'structure','contours'} for each volume colormaps - cell array of colormaps (e.g., {'gray','jet'}) slices - vector of slice indices (e.g. [20 30 40]) sliceType - 'axial','coronal','sagittal' Example: vol1 = rand(50,50,50); vol2 = rand(50,50,50) > 0.7; whifun_multiOverlay({vol1,vol2},{'structure','contours'},{'gray','jet'},[10 20 30],'axial'); % --- Load Volumes ---
- **Arguments:**
  - `volumes` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `overlayTypes` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `colormaps` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slices` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `sliceType` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB NIfTI I/O
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.
