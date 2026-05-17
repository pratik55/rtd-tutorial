# Module Name: `whifun_functions/load_subjects_all.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - LOAD_SUBJECTS_ALL Loads all subjects from a CSV file, with options for new runs. Subj_list_all = LOAD_SUBJECTS_ALL(folder, name) loads all subjects from a CSV file without any filtering. The function reads the CSV file named 'name' from the specified 'folder' and returns the data as a structure array. Subj_list_all = LOAD_SUBJECTS_ALL(folder, name, new_run) allows you to initialize the file for a new data run. - If `new_run` is true (1), the function adds 'error' and 'motion_ex' columns and initializes them to zeros. This is useful for starting a new analysis where you need to track errors and
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O

## Function: `load_subjects_all()`
- **Signature & Definition:** `function Subj_list_all = load_subjects_all(folder,name,new_run,overwrite)` (line 1)
- **Scientific Theory & Formulas:** Band-pass filtering uses Butterworth IIR coefficients; forward-backward `filtfilt` cancels phase delay and squares the magnitude response. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** LOAD_SUBJECTS_ALL Loads all subjects from a CSV file, with options for new runs. Subj_list_all = LOAD_SUBJECTS_ALL(folder, name) loads all subjects from a CSV file without any filtering. The function reads the CSV file named 'name' from the specified 'folder' and returns the data as a structure array. Subj_list_all = LOAD_SUBJECTS_ALL(folder, name, new_run) allows you to initialize the file for a new data run. - If `new_run` is true (1), the function adds 'error' and 'motion_ex' columns and initializes them to zeros. This is useful for starting a new analysis where you need to track errors and exclusions. Subj_list_all = LOAD_SUBJECTS_ALL(folder, name, new_run, overwrite) provides an option 
- **Arguments:**
  - `folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `name` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `new_run` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `overwrite` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Subj_list_all` (structure array containing participant metadata and paths): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB table/file I/O
  - Called By: `main.mlapp:1026/RunDataCheckButtonPushed`, `main.mlapp:1538/ExtractROITImeseriesButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2138/DetermineFramewiseDisplacementthresholdsButtonPushed`, `main.mlapp:2169/DeletePreprocessingfilesfromaparticularstepButtonPushed`, `main.mlapp:2323/ManuallyexcludeparticipantsCheckBoxValueChanged`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_get_common_subjects.m:1/whifun_get_common_subjects`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`, `whifun_functions/whifun_using_other_preproc.m:1/whifun_using_other_preproc`, `whifun_functions/whifun_using_other_preproc_segment_fsl.m:1/whifun_using_other_preproc_segment_fsl`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Emits warnings for recoverable conditions.
