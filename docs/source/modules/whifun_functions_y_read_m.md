# Module Name: `whifun_functions/y_Read.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - function [Data, Header] = y_Read(FileName, VolumeIndex) Read NIfTI file Based on SPM's nifti ------------------------------------------------------------------------ Input: FileName - the path and filename of the image file (*.img, *.hdr, *.nii, *.nii.gz) VolumeIndex - the index of one volume within the 4D data to be read, can be 1,2,..., or 'all'. default: 'all' - means read all volumes Output: Data - 3D or 4D matrix of image data Header - a structure containing image volume information (as defined by SPM, see spm_vol.m) The elements in the structure are: Header.fname - the filename of the im
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: SPM12

## Function: `y_Read()`
- **Signature & Definition:** `function [Data, Header] = y_Read(FileName, VolumeIndex)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** function [Data, Header] = y_Read(FileName, VolumeIndex) Read NIfTI file Based on SPM's nifti ------------------------------------------------------------------------ Input: FileName - the path and filename of the image file (*.img, *.hdr, *.nii, *.nii.gz) VolumeIndex - the index of one volume within the 4D data to be read, can be 1,2,..., or 'all'. default: 'all' - means read all volumes Output: Data - 3D or 4D matrix of image data Header - a structure containing image volume information (as defined by SPM, see spm_vol.m) The elements in the structure are: Header.fname - the filename of the image. Header.dim - the x, y and z dimensions of the volume Header.dt - A 1x2 array. First element is 
- **Arguments:**
  - `FileName` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `VolumeIndex` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `Data` (numeric scalar, vector, matrix, or multidimensional array): Output produced by the MATLAB implementation.
  - `Header` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: SPM12
  - Called By: `whifun_functions/reslice_data.m:1/reslice_data`, `whifun_functions/save_mat_to_nifti.m:1/save_mat_to_nifti`, `whifun_functions/whifun_get_ts_from_mask.m:1/whifun_get_ts_from_mask`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.
