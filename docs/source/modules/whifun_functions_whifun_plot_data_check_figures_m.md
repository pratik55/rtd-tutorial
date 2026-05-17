# Module Name: `whifun_functions/whifun_plot_data_check_figures.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_PLOT_DATA_CHECK_FIGURES Generates and saves quality control figures summarizing scanning parameters (time points, TR, and voxel sizes) across all participants. WHIFUN_PLOT_DATA_CHECK_FIGURES(QUALITY_CONTROL_PATH, N_IMAGE, TR, VOXEL_FUNC, VOXEL_ANAT, MIS_DATA) This function creates two figures: 1. Bar plots of scanning parameters for each participant. 2. Histograms of scanning parameters to check for homogeneity across the group. Input Arguments: QUALITY_CONTROL_PATH - The directory where the output figures will be saved. N_IMAGE - Vector containing the number of fMRI time points for eac
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: ANTs command-line suite

## Function: `whifun_plot_data_check_figures()`
- **Signature & Definition:** `function whifun_plot_data_check_figures(quality_control_path,n_image,tr,voxel_func,voxel_anat,mis_data)` (line 1)
- **Scientific Theory & Formulas:** Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_PLOT_DATA_CHECK_FIGURES Generates and saves quality control figures summarizing scanning parameters (time points, TR, and voxel sizes) across all participants. WHIFUN_PLOT_DATA_CHECK_FIGURES(QUALITY_CONTROL_PATH, N_IMAGE, TR, VOXEL_FUNC, VOXEL_ANAT, MIS_DATA) This function creates two figures: 1. Bar plots of scanning parameters for each participant. 2. Histograms of scanning parameters to check for homogeneity across the group. Input Arguments: QUALITY_CONTROL_PATH - The directory where the output figures will be saved. N_IMAGE - Vector containing the number of fMRI time points for each participant. TR - Vector containing the Repetition Time (TR) for each participant. VOXEL_FUNC - Ma
- **Arguments:**
  - `quality_control_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `n_image` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `tr` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `voxel_func` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `voxel_anat` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mis_data` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: ANTs command-line suite
  - Called By: `main.mlapp:1026/RunDataCheckButtonPushed`, `whifun_functions/whifun_create_qc.m:1/whifun_create_qc`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.
