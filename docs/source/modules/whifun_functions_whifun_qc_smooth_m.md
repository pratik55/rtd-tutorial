# Module Name: `whifun_functions/whifun_qc_smooth.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_SMOOTH Generates a quality control image for spatial smoothing. WHIFUN_QC_SMOOTH(out_folder, func_image, slover_slices_ss, slover_contour_range_ss, slover_view, over_write) creates a visual quality control report to assess the effect of spatial smoothing on a functional image. The function performs the following steps: 1. **File Management**: It checks for the existence of previous quality control images (both orthoslice and slover views). Based on the `over_write` flag, it determines whether to generate new plots. It also creates the necessary output directories if they don't exist.
  - Internal calls detected: `whifun_create_file`, `whifun_ortho_slover_single_image_save`
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## `whifun_qc_smooth()`

### Syntax
```matlab
function whifun_qc_smooth(out_folder,func_image,name,slover_slices_ss,slover_contour_range_ss,slover_view,over_write)
```
Defined at source line `1`.

### Description
WHIFUN_QC_SMOOTH Generates a quality control image for spatial smoothing. WHIFUN_QC_SMOOTH(out_folder, func_image, slover_slices_ss, slover_contour_range_ss, slover_view, over_write) creates a visual quality control report to assess the effect of spatial smoothing on a functional image. The function performs the following steps: 1. **File Management**: It checks for the existence of previous quality control images (both orthoslice and slover views). Based on the `over_write` flag, it determines whether to generate new plots. It also creates the necessary output directories if they don't exist. 2. **Plotting**: It calls a helper function, `whifun_ortho_slover_single_image_save`, to generate t

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `out_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `func_image` — numeric image/header data, commonly X x Y x Z or X x Y x Z x T
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_slices_ss` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_contour_range_ss` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `slover_view` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `over_write` — logical or numeric flag
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Checks empty arrays, missing files, or empty user selections.

### Algorithms
Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_ortho_slover_single_image_save`
- **External Dependencies:** SLover/MarsBaR-style visualization helpers
- **Called By:** `whifun_functions/whifun_qc.m:1/whifun_qc`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_ortho_slover_single_image_save`
- Related callers: `whifun_functions/whifun_qc.m:1/whifun_qc`
