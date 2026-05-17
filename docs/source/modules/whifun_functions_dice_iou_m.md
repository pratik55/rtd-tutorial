# Module Name: `whifun_functions/dice_iou.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Key Features:**
  - DICE_IOU Computes the Dice Similarity Coefficient and Intersection of Union (IoU) between two functional network (FN) atlas NIfTI files. It can optionally align the second network to the first and generate a visualization of the similarity matrix. [DICE, IOU, VOX_NUM_1, VOX_NUM_2] = DICE_IOU(KMEANS_NET_1_PATH, KMEANS_NET_2_PATH, ALIGN_NET, FIG_DICE) Input Arguments: KMEANS_NET_1_PATH - Full path to the first FN NIfTI file, or the N-dimensional array itself. KMEANS_NET_2_PATH - Full path to the second FN NIfTI file, or the N-dimensional array itself. ALIGN_NET - (Optional, default 0) Flag to al
  - Internal calls detected: `niftisave`, `whifun_convert_3d_to_4d_atlas`
  - External dependencies detected: MATLAB NIfTI I/O

## Function: `dice_iou()`
- **Signature & Definition:** `function [dice,IOU,vox_num_1,vox_num_2] = dice_iou(kmeans_net_1_path,kmeans_net_2_path,align_net,fig_dice)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Data-management code preserves participant provenance, BIDS/custom path mapping, and reproducible bookkeeping.
- **Functional Purpose:** DICE_IOU Computes the Dice Similarity Coefficient and Intersection of Union (IoU) between two functional network (FN) atlas NIfTI files. It can optionally align the second network to the first and generate a visualization of the similarity matrix. [DICE, IOU, VOX_NUM_1, VOX_NUM_2] = DICE_IOU(KMEANS_NET_1_PATH, KMEANS_NET_2_PATH, ALIGN_NET, FIG_DICE) Input Arguments: KMEANS_NET_1_PATH - Full path to the first FN NIfTI file, or the N-dimensional array itself. KMEANS_NET_2_PATH - Full path to the second FN NIfTI file, or the N-dimensional array itself. ALIGN_NET - (Optional, default 0) Flag to align net_2 to net_1: ALIGN_NET = 1: Relabels net_2 based on the maximum Dice match to net_1 and saves
- **Arguments:**
  - `kmeans_net_1_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `kmeans_net_2_path` (character vector or string scalar filesystem path): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `align_net` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `fig_dice` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `dice` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `IOU` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `vox_num_1` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
  - `vox_num_2` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: `niftisave`, `whifun_convert_3d_to_4d_atlas`
  - External: MATLAB NIfTI I/O
  - Called By: `main.mlapp:1480/CompareFNButtonPushed`, `main.mlapp:417/get_symettry_indi`, `whifun_functions/get_symettry_indi.m:1/get_symettry_indi`, `whifun_functions/whifun_compute_stability.m:1/whifun_compute_stability`
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files.
