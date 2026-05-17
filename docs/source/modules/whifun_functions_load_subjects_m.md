# Module Name: `whifun_functions/load_subjects.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - LOAD_SUBJECTS Loads a list of subjects from a CSV file. [Subj_list, rm] = LOAD_SUBJECTS(folder, name) loads a CSV file named 'name' from the specified 'folder'. It returns a structure array 'Subj_list' containing the subject data and a logical array 'rm' indicating which rows were removed. The function automatically removes subjects marked with 'error', 'motion_ex', or 'manual_ex'. [Subj_list, rm] = LOAD_SUBJECTS(folder, name, first) allows for different behavior on the first run. If 'first' is true (1), the function initializes new 'error' and 'motion_ex' columns with zeros and only removes s
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O

## Function: `load_subjects()`
- **Signature & Definition:** `function [Subj_list,rm] = load_subjects(folder,name,first)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** LOAD_SUBJECTS Loads a list of subjects from a CSV file. [Subj_list, rm] = LOAD_SUBJECTS(folder, name) loads a CSV file named 'name' from the specified 'folder'. It returns a structure array 'Subj_list' containing the subject data and a logical array 'rm' indicating which rows were removed. The function automatically removes subjects marked with 'error', 'motion_ex', or 'manual_ex'. [Subj_list, rm] = LOAD_SUBJECTS(folder, name, first) allows for different behavior on the first run. If 'first' is true (1), the function initializes new 'error' and 'motion_ex' columns with zeros and only removes subjects marked with 'manual_ex'. This is useful for initial data processing runs. Input Arguments: f
- **Arguments:**
  - `folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `name` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `first` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
  - `rm` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB table/file I/O
  - Called By: `Sub_info.mlapp:142/ParticipantsgoodtopreprocessButtonPushed`, `main.mlapp:1026/RunDataCheckButtonPushed`, `main.mlapp:1223/CreateGroupMasksButtonPushed`, `main.mlapp:1298/CreateWMFNButtonPushed`, `main.mlapp:1408/CreateGMFNButtonPushed`, `main.mlapp:1457/StatisticsButtonPushed`, `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1831/QCcheckdoneCheckBoxValueChanged`, `main.mlapp:204/load_param`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:2323/ManuallyexcludeparticipantsCheckBoxValueChanged`, `main.mlapp:2486/CreateWMGMFNButtonPushed`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Handles NaN, Inf, or finite-value filtering. Emits warnings for recoverable conditions.
