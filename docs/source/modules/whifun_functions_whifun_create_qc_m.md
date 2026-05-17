# Module Name: `whifun_functions/whifun_create_qc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - if ~only_check_data %% for subji = 1:length(Subj_list) disp('..') disp(['Currently Processing ' Subj_list(subji).name]) Subj_list_1 = Subj_list(subji); motion_txt = load(complete_filepath(['C:\Users\jainp\Box\practice_NYU_abide\' Subj_list_1.name '\session_1\rest_1\rp_*.txt'])); whifun_qc(quality_control_path,Subj_list_1,'motion_txt',motion_txt); end end
  - Internal calls detected: `whifun_check_data`, `whifun_create_Subj_list`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`
  - External dependencies detected: MATLAB table/file I/O

## Function: `whifun_create_qc()`
- **Signature & Definition:** `function Subj_list = whifun_create_qc` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** if ~only_check_data %% for subji = 1:length(Subj_list) disp('..') disp(['Currently Processing ' Subj_list(subji).name]) Subj_list_1 = Subj_list(subji); motion_txt = load(complete_filepath(['C:\Users\jainp\Box\practice_NYU_abide\' Subj_list_1.name '\session_1\rest_1\rp_*.txt'])); whifun_qc(quality_control_path,Subj_list_1,'motion_txt',motion_txt); end end
- **Arguments:**
  - No explicit input arguments.
- **Returns:**
  - `Subj_list` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_check_data`, `whifun_create_Subj_list`, `whifun_isnan_or_empty`, `whifun_plot_data_check_figures`
  - External: MATLAB table/file I/O
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Handles NaN, Inf, or finite-value filtering.
