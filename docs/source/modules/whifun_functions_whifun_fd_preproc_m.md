# Module Name: `whifun_functions/whifun_fd_preproc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_FD_PREPROC Performs quality control based on framewise displacement. Subj_list_1 = WHIFUN_FD_PREPROC(quality_control_path, Subj_list_1, ..., greater_than_20) calculates the framewise displacement (FD) and assesses whether a subject's head motion exceeds predefined quality control thresholds. The function first computes the FD using the motion parameters. It then applies three checks: 1. **Maximum FD**: Is the maximum FD value greater than `max_fd`? 2. **Mean FD**: Is the mean FD value greater than `mean_fd`? 3. **Percentage of high-motion volumes**: Is the percentage of volumes with FD 
  - Internal calls detected: `whifun_calculate_fd`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_fd_preproc()`
- **Signature & Definition:** `function Subj_list_1 = whifun_fd_preproc(quality_control_path,Subj_list_1,in_motion_txt_path,max_fd,mean_fd,greater_than_20)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_FD_PREPROC Performs quality control based on framewise displacement. Subj_list_1 = WHIFUN_FD_PREPROC(quality_control_path, Subj_list_1, ..., greater_than_20) calculates the framewise displacement (FD) and assesses whether a subject's head motion exceeds predefined quality control thresholds. The function first computes the FD using the motion parameters. It then applies three checks: 1. **Maximum FD**: Is the maximum FD value greater than `max_fd`? 2. **Mean FD**: Is the mean FD value greater than `mean_fd`? 3. **Percentage of high-motion volumes**: Is the percentage of volumes with FD greater than `greater_than_20` more than 20%? If any of these conditions are met, the subject is fla
- **Arguments:**
  - `quality_control_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_1` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `in_motion_txt_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `max_fd` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `mean_fd` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `greater_than_20` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_1` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_calculate_fd`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`, `whifun_functions/whifun_post_proc_hcp.m:1/whifun_post_proc_hcp`, `whifun_functions/whifun_post_proc_hcp_dev.m:1/whifun_post_proc_hcp_dev`, `whifun_functions/whifun_preproc.m:1/whifun_preproc`, `whifun_functions/whifun_preproc_fsl.m:1/whifun_preproc_fsl`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.
