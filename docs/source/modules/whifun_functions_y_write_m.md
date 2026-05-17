# Module Name: `whifun_functions/y_Write.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - Write NIfTI file (3D or 4D) Based on SPM's nifti or Write GIfTI file (1D or 2D) Based on SPM's gifti or Write DPABINet Matrix files %------------------------------------------------------------------------ 1. For NIfTI Write data (Data) with a specified header (Header) into a image file with format of Nifti 1.1. The data (Data) should be 3D or 4D matrix, the header (Header) should be a structure the same as SPM. If the filename (OutName) is with extra name as '.img', then it will generate two files (header and data seperately), or else, '.nii', it will generate single file with header and data
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB table/file I/O, SPM12

## Function: `y_Write()`
- **Signature & Definition:** `function y_Write(Data,Header,OutName)` (line 1)
- **Scientific Theory & Formulas:** Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** Write NIfTI file (3D or 4D) Based on SPM's nifti or Write GIfTI file (1D or 2D) Based on SPM's gifti or Write DPABINet Matrix files %------------------------------------------------------------------------ 1. For NIfTI Write data (Data) with a specified header (Header) into a image file with format of Nifti 1.1. The data (Data) should be 3D or 4D matrix, the header (Header) should be a structure the same as SPM. If the filename (OutName) is with extra name as '.img', then it will generate two files (header and data seperately), or else, '.nii', it will generate single file with header and data together. Usage: y_Write(Data,Header,OutName) Input: 1) Data - Data of 4D matrix to write 2) Header
- **Arguments:**
  - `Data` (numeric scalar, vector, matrix, or multidimensional array): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `Header` (numeric image/header data, commonly X x Y x Z or X x Y x Z x T): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `OutName` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: MATLAB table/file I/O, SPM12
  - Called By: `whifun_functions/reslice_data.m:1/reslice_data`, `whifun_functions/save_mat_to_nifti.m:1/save_mat_to_nifti`
- **Edge Cases & Exceptions:** Uses try/catch; failures are logged, displayed, or returned. Checks empty arrays, missing files, or empty user selections.
