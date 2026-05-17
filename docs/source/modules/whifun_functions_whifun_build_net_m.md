# Module Name: `whifun_functions/whifun_build_net.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_BUILD_NET Manages the decision process for building Functional Networks (FNs). [BUILD_NET, K] = WHIFUN_BUILD_NET(CLUSTER_FOLDER, OUT_PATTERN, OVER_WRITE) This function checks if previously clustered FN files exist in the specified folder. If files are found, it prompts the user to either rebuild the networks or select an existing cluster solution (K value) to proceed with. Input Arguments: CLUSTER_FOLDER - Full path to the directory where FN cluster results are stored. OUT_PATTERN - The filename pattern used for the clustered NIfTI files (e.g., 'WM_FN_K*.nii', where * is the K value). O
  - Internal calls detected: `whifun_create_file`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_build_net()`
- **Signature & Definition:** `function [build_net,K] = whifun_build_net(cluster_folder,out_pattern,over_write)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_BUILD_NET Manages the decision process for building Functional Networks (FNs). [BUILD_NET, K] = WHIFUN_BUILD_NET(CLUSTER_FOLDER, OUT_PATTERN, OVER_WRITE) This function checks if previously clustered FN files exist in the specified folder. If files are found, it prompts the user to either rebuild the networks or select an existing cluster solution (K value) to proceed with. Input Arguments: CLUSTER_FOLDER - Full path to the directory where FN cluster results are stored. OUT_PATTERN - The filename pattern used for the clustered NIfTI files (e.g., 'WM_FN_K*.nii', where * is the K value). OVER_WRITE - (Optional, default 0) Flag to bypass prompts if set to 1. Output Arguments: BUILD_NET - 
- **Arguments:**
  - `cluster_folder` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `out_pattern` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `over_write` (logical or numeric flag): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `build_net` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `K` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `whifun_create_file`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_create_FN_Kmeans.m:1/whifun_create_FN_Kmeans`, `whifun_functions/whifun_create_FN_Kmeans_WM_GM.m:1/whifun_create_FN_Kmeans_WM_GM`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. May pause for interactive user input, which affects batch reproducibility.
