# Module Name: `whifun_functions/whifun_compute_stability.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - WHIFUN_COMPUTE_STABILITY Calculates the stability of Functional Networks (FNs) using the average maximum Dice similarity coefficient across all unique pairwise comparisons of network maps. [AVG_MAX_DICE, DICEIJ_ALL, VOX_NUM_ALL] = WHIFUN_COMPUTE_STABILITY(NET_LIST, NET_INCLUDE) This is typically used in cross-validation/bootstrapping steps of FN creation (e.g., k-means clustering) to assess how consistently networks are identified across different partitions of the data. Input Arguments: NET_LIST - A structure array (e.g., from MATLAB's `dir` function) where each element points to a NIfTI file
  - Internal calls detected: `dice_iou`
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_compute_stability()`
- **Signature & Definition:** `function [avg_max_dice,diceij_all,vox_num_all] = whifun_compute_stability(net_list,net_include)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** WHIFUN_COMPUTE_STABILITY Calculates the stability of Functional Networks (FNs) using the average maximum Dice similarity coefficient across all unique pairwise comparisons of network maps. [AVG_MAX_DICE, DICEIJ_ALL, VOX_NUM_ALL] = WHIFUN_COMPUTE_STABILITY(NET_LIST, NET_INCLUDE) This is typically used in cross-validation/bootstrapping steps of FN creation (e.g., k-means clustering) to assess how consistently networks are identified across different partitions of the data. Input Arguments: NET_LIST - A structure array (e.g., from MATLAB's `dir` function) where each element points to a NIfTI file containing the labeled Functional Network map for a specific data fold. NET_INCLUDE - (Optional, de
- **Arguments:**
  - `net_list` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `net_include` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `avg_max_dice` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `diceij_all` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `vox_num_all` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `dice_iou`
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections.
