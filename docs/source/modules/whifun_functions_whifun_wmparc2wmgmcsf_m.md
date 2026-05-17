# Module Name: `whifun_functions/whifun_wmparc2wmgmcsf.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Tissue masks use label or probability thresholding. Group consensus includes voxel $v$ when $S^{-1}\sum_s I_s(v)\ge\tau$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - separate_tissues.m This script separates a loaded brain segmentation matrix into three separate binary matrices for White Matter (WM), Gray Matter (GM), and Cerebrospinal Fluid (CSF) based on standard FreeSurfer labels. Assumes the wmparc.nii.gz file is already loaded into a 3D matrix, for example, using a command like:
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: MATLAB NIfTI I/O
