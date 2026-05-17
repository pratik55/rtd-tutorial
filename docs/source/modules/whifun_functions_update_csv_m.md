# Module Name: `whifun_functions/update_csv.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - UPDATE_CSV Updates Subj_list structure with new information for a specific subject and saves the entire list to a CSV file. SUBJ_LIST_ALL = UPDATE_CSV(SUBJ_LIST_SUBJI, SUBJ_LIST_ALL, OUTPUT_FOLDER) This utility function is typically used in a processing pipeline to record the status and results (e.g., motion metrics, processing time, error flags) for one subject into the complete subject list. Input Arguments: SUBJ_LIST_SUBJI - A structure representing a single subject, containing the updated fields to be transferred (e.g., `motion_ex`, `error`, `nt_dis`, `time_preprocess_min`). Must have a `n
  - Internal calls detected: `my_writetable`
  - External dependencies detected: MATLAB table/file I/O

## Function: `update_csv()`
- **Signature & Definition:** `function Subj_list_all = update_csv(Subj_list_subji,Subj_list_all,output_folder)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** UPDATE_CSV Updates Subj_list structure with new information for a specific subject and saves the entire list to a CSV file. SUBJ_LIST_ALL = UPDATE_CSV(SUBJ_LIST_SUBJI, SUBJ_LIST_ALL, OUTPUT_FOLDER) This utility function is typically used in a processing pipeline to record the status and results (e.g., motion metrics, processing time, error flags) for one subject into the complete subject list. Input Arguments: SUBJ_LIST_SUBJI - A structure representing a single subject, containing the updated fields to be transferred (e.g., `motion_ex`, `error`, `nt_dis`, `time_preprocess_min`). Must have a `name` field for matching. SUBJ_LIST_ALL - The master structure array containing data for all subjects
- **Arguments:**
  - `Subj_list_subji` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Subj_list_all` (structure array containing participant metadata and paths): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `output_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `my_writetable`
  - External: MATLAB table/file I/O
  - Called By: `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.
