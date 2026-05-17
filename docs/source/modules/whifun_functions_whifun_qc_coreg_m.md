# Module Name: `whifun_functions/whifun_qc_coreg.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_QC_COREG Generates quality control images for coregistration. WHIFUN_QC_COREG(out_folder, func_image_path, anat_image_path, name, slover_slices_ss, slover_contour_range_ss, slover_view, over_write) creates visual quality control reports to assess the alignment of a subject's functional data to their anatomical data after coregistration. The function generates two types of plots to check the alignment: 1. **SPM Orthoslice Plot**: It calls `whifun_qc_coreg_orthoslice` to generate a plot using SPM's `check_registration`. The skull-stripped anatomical image is used as the underlay, and the 
  - Internal calls detected: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`
  - External dependencies detected: SLover/MarsBaR-style visualization helpers

## Function: `whifun_qc_coreg()`
- **Signature & Definition:** `function whifun_qc_coreg(out_folder,func_image_path,anat_image_path,name,slover_slices_ss,slover_contour_range_ss,slover_view,over_write)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Registration uses affine coordinates $x_{world}=M[x\;1]$ and, for normalization, deformation fields; SPM coregistration uses normalized mutual information for multimodal alignment. Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_QC_COREG Generates quality control images for coregistration. WHIFUN_QC_COREG(out_folder, func_image_path, anat_image_path, name, slover_slices_ss, slover_contour_range_ss, slover_view, over_write) creates visual quality control reports to assess the alignment of a subject's functional data to their anatomical data after coregistration. The function generates two types of plots to check the alignment: 1. **SPM Orthoslice Plot**: It calls `whifun_qc_coreg_orthoslice` to generate a plot using SPM's `check_registration`. The skull-stripped anatomical image is used as the underlay, and the first volume of the realigned functional image is used as an overlay. This plot allows for a quick v
- **Arguments:**
  - `out_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `func_image_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `anat_image_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `name` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_slices_ss` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_contour_range_ss` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `slover_view` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: `whifun_create_file`, `whifun_qc_coreg_orthoslice`, `whifun_qc_coreg_slover`
  - External: SLover/MarsBaR-style visualization helpers
  - Called By: `whifun_functions/whifun_qc.m:1/whifun_qc`
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.
