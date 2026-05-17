# Module Name: `whifun_functions/whifun_copyfiles.m`

## Description
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - whifun_copyfiles(Subj_list, field_name, dest_folder) Copies files listed in a specified field of a struct array to a destination folder, preserving their directory structure relative to their source locations. Example: whifun_copyfiles(Subj_list, 'func_path', 'D:\All_Func_Files') Inputs: Subj_list : Struct array (e.g., Subj_list(i).func_path = '/data/sub1/func.nii') field_name : Name of the field containing file paths dest_folder : Destination root folder for copied files Notes: - Creates subfolders as needed to mirror the source directory structure. - Keeps original filenames. - Assumes all f
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## `whifun_copyfiles()`

### Syntax
```matlab
function whifun_copyfiles(Subj_list, field_name, dest_folder)
```
Defined at source line `1`.

### Description
whifun_copyfiles(Subj_list, field_name, dest_folder) Copies files listed in a specified field of a struct array to a destination folder, preserving their directory structure relative to their source locations. Example: whifun_copyfiles(Subj_list, 'func_path', 'D:\All_Func_Files') Inputs: Subj_list : Struct array (e.g., Subj_list(i).func_path = '/data/sub1/func.nii') field_name : Name of the field containing file paths dest_folder : Destination root folder for copied files Notes: - Creates subfolders as needed to mirror the source directory structure. - Keeps original filenames. - Assumes all files share a common root (e.g., '/data'). You can customize the 'common_root' detection below if nee

### Examples
No runnable examples were extracted during the source-static review for this function.

### Input Arguments
#### `Subj_list` — structure array containing participant metadata and paths
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `field_name` — character vector, string scalar, or categorical option
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

#### `dest_folder` — character vector or string scalar filesystem path
Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.

### Name-Value Arguments
No explicit name-value arguments were documented in the source-static review for this function.

### Output Arguments
- No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.

### More About
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Tips
Defines defaults or branches for optional arguments or missing files. Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections. Emits warnings for recoverable conditions. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.

### Algorithms
Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.

### Extended Capabilities
- **Internal Calls:** No internal WhiFuN calls detected in this function body.
- **External Dependencies:** No major external dependency pattern detected beyond MATLAB base language.
- **Called By:** No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.

### Version History
- Source-static review snapshot date: `2026-05-16`.
- Runtime execution of MATLAB code was not performed during documentation generation.

### See Also
No related internal cross-references were documented in the source-static review.
