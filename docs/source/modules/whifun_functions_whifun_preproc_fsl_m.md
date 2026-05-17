# Module Name: `whifun_functions/whifun_preproc_fsl.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_PREPROC_FSL Comprehensive FSL-based fMRI preprocessing pipeline. SUBJ_LIST_1 = WHIFUN_PREPROC_FSL(QC_PATH, SUBJ_STRUCT, 'Name', Value) executes a full preprocessing workflow for a single subject, including volume discarding, motion correction (MCFLIRT), FD calculation, anatomical processing (fsl_anat), normalization to MNI space, nuisance regression, and spatial smoothing. INPUTS: quality_control_path - String. Path to the directory where logs and QC outputs will be stored. Subj_list_1 - Struct. Contains subject-specific fields: .name : Subject ID .func_folder : Path to functional data
  - Internal calls detected: `whifun_create_file`, `whifun_create_rest_mask`, `whifun_csf_mask_extraction_preproc`, `whifun_discard_initial_volume_preproc`, `whifun_extract_csf_ts_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_nuisance_regress_preproc`, `whifun_smooth_preproc`
  - External dependencies detected: MATLAB table/file I/O, SPM12, FSL command-line suite, Shell/system execution

## `whifun_preproc_fsl()`

### Syntax
```matlab
function Subj_list_1 = whifun_preproc_fsl(quality_control_path, Subj_list_1, varargin)
```
Defined at source line `1`.

### Description
WHIFUN_PREPROC_FSL Comprehensive FSL-based fMRI preprocessing pipeline. SUBJ_LIST_1 = WHIFUN_PREPROC_FSL(QC_PATH, SUBJ_STRUCT, 'Name', Value) executes a full preprocessing workflow for a single subject, including volume discarding, motion correction (MCFLIRT), FD calculation, anatomical processing (fsl_anat), normalization to MNI space, nuisance regression, and spatial smoothing. INPUTS: quality_control_path - String. Path to the directory where logs and QC outputs will be stored. Subj_list_1 - Struct. Contains subject-specific fields: .name : Subject ID .func_folder : Path to functional data .func_name : Name of functional NIfTI .anat_folder : Path to anatomical data .anat_name : Name of an

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `quality_control_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `Subj_list_1` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `varargin` — cell array of variable MATLAB arguments
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `Subj_list_1` — structure array containing participant metadata and paths
Output produced by the MATLAB implementation.

### More About
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Uses explicit parameter parsing or validation. Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands. Depends on external command availability and shell exit status.

### Algorithms
Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Gaussian smoothing uses $G_\sigma(x)=\frac{1}{(2\pi\sigma^2)^{3/2}}e^{-\lVert x\rVert^2/(2\sigma^2)}$ and $\sigma=\mathrm{FWHM}/(2\sqrt{2\ln2})$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** `whifun_create_file`, `whifun_create_rest_mask`, `whifun_csf_mask_extraction_preproc`, `whifun_discard_initial_volume_preproc`, `whifun_extract_csf_ts_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_nuisance_regress_preproc`, `whifun_smooth_preproc`
- **External Dependencies:** MATLAB table/file I/O, SPM12, FSL command-line suite, Shell/system execution
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related internal calls: `whifun_create_file`, `whifun_create_rest_mask`, `whifun_csf_mask_extraction_preproc`, `whifun_discard_initial_volume_preproc`, `whifun_extract_csf_ts_preproc`, `whifun_fd_preproc`, `whifun_fsl_fast_seg`, `whifun_nuisance_regress_preproc`, `whifun_smooth_preproc`
