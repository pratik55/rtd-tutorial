# Module Name: `uigetfile_n_dir/uigetfile_n_dir.m`

## Description
- **Module Category:** Bundled file-selection helper.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Pick multiple directories and/or files
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `uigetfile_n_dir()`

### Syntax
```matlab
function [pathname] = uigetfile_n_dir(start_path, dialog_title)
```
Defined at source line `1`.

### Description
Pick multiple directories and/or files

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `start_path` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `dialog_title` — MATLAB value inferred from source usage
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
#### `pathname` — character vector or string scalar filesystem path
Output produced by the MATLAB implementation.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:2323/ManuallyexcludeparticipantsCheckBoxValueChanged`, `rerunpreproc.mlapp:358/SelectParticipantsButtonPushed`, `whifun_display_FC.mlapp:1584/Group1ParticipantsSelectButtonPushed`, `whifun_display_FC.mlapp:1624/Group2ParticipantsSelectButtonPushed`

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
- Related callers: `main.mlapp:1656/SelectParticipantsButtonPushed`, `main.mlapp:2216/AllfoldersareParticipantsCheckBoxValueChanged`, `main.mlapp:2323/ManuallyexcludeparticipantsCheckBoxValueChanged`, `rerunpreproc.mlapp:358/SelectParticipantsButtonPushed`, `whifun_display_FC.mlapp:1584/Group1ParticipantsSelectButtonPushed`, `whifun_display_FC.mlapp:1624/Group2ParticipantsSelectButtonPushed`
