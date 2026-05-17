# Module Name: `whifun_functions/whifun_select_confound_vars.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.
- **Key Features:**
  - WHIFUN_SELECT_CONFOUND_VARS Select confound variables using wildcard patterns (*) INPUTS confound_vars : cell array of char or string Reg_params : cell array of patterns (e.g., {'csf','aroma*','*motion*'}) OUTPUT selected_vars : cell array of matched confound variable names Ensure cell array of char
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_select_confound_vars()`
- **Signature & Definition:** `function idx_all = whifun_select_confound_vars(confound_vars, Reg_params)` (line 1)
- **Scientific Theory & Formulas:** Linear models use $y=X\beta+\varepsilon$; residualized data are $\hat{\varepsilon}=y-X\hat{\beta}$, with temporal means often added back. Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$.
- **Functional Purpose:** WHIFUN_SELECT_CONFOUND_VARS Select confound variables using wildcard patterns (*) INPUTS confound_vars : cell array of char or string Reg_params : cell array of patterns (e.g., {'csf','aroma*','*motion*'}) OUTPUT selected_vars : cell array of matched confound variable names Ensure cell array of char
- **Arguments:**
  - `confound_vars` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Reg_params` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `idx_all` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_post_preproc_fmriprep.m:1/whifun_post_preproc_fmriprep`
- **Edge Cases & Exceptions:** Checks empty arrays, missing files, or empty user selections.
