# Module Name: `whifun_functions/whifun_dir.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_DIR Safely retrieves directory information. This function wraps the standard MATLAB dir command in a try-catch block. It is particularly useful for robustly handling missing directories or path-string errors without interrupting the execution of a larger preprocessing loop. INPUTS: path_ - String or Character array. The path or file pattern to be listed (e.g., '/data/sub-*/func/'). OUTPUTS: out - A structure array containing directory information. Returns an empty array [] if the path is invalid or an error occurs. EXAMPLE: % Safely check for the presence of a specific session contents 
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_dir()`
- **Signature & Definition:** `function out = whifun_dir(path_)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_DIR Safely retrieves directory information. This function wraps the standard MATLAB dir command in a try-catch block. It is particularly useful for robustly handling missing directories or path-string errors without interrupting the execution of a larger preprocessing loop. INPUTS: path_ - String or Character array. The path or file pattern to be listed (e.g., '/data/sub-*/func/'). OUTPUTS: out - A structure array containing directory information. Returns an empty array [] if the path is invalid or an error occurs. EXAMPLE: % Safely check for the presence of a specific session contents = whifun_dir(fullfile(subj_dir, 'ses-02')); if isempty(contents) fprintf('Session 02 not found for t
- **Arguments:**
  - `path_` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `out` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:1774/DataPathTextAreaValueChanged`, `main.mlapp:1895/manuallycoregisterparticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:550/ParticipantDatafolderButtonPushed`, `main.mlapp:616/RunPreprocessingButtonPushed`, `whifun_functions/whifun_preproc_all.m:1/whifun_preproc_all`
- **Edge Cases & Exceptions:** Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions.
