# Module Name: `whifun_functions/whifun_plot_dice_coef_and_elb.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Key Features:**
  - WHIFUN_PLOT_DICE_COEF_AND_ELB Plots the Dice Coefficient and Distortion (ELBO proxy) over a range of K-values. WHIFUN_PLOT_DICE_COEF_AND_ELB(DICE_COEFFICIENT_FOLDS_ALL, ELB, K_RANGE_L, K_RANGE_H) generates a plot showing the trend of the Dice Coefficient and a proxy for the Evidence Lower Bound (ELB/Distortion) across different K-values (e.g., number of clusters). Input Arguments: DICE_COEFFICIENT_FOLDS_ALL - A vector containing the mean Dice Coefficients for each K-value. ELB - A vector containing the corresponding Distortion (or ELBO proxy) values for each K-value. K_RANGE_L - The lowest K-v
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_plot_dice_coef_and_elb()`
- **Signature & Definition:** `function whifun_plot_dice_coef_and_elb(Dice_coefficient_folds_all,elb,K_range_l,K_range_h)` (line 1)
- **Scientific Theory & Formulas:** K-means minimizes $\sum_i \lVert x_i-\mu_{c_i}\rVert_d^2$; WhiFuN uses correlation-distance voxel-connectivity features for FN maps. Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$. Visualization modules use slice sampling, overlays, contours, colormaps, and surface or graph rendering without adding a separate inferential model.
- **Functional Purpose:** WHIFUN_PLOT_DICE_COEF_AND_ELB Plots the Dice Coefficient and Distortion (ELBO proxy) over a range of K-values. WHIFUN_PLOT_DICE_COEF_AND_ELB(DICE_COEFFICIENT_FOLDS_ALL, ELB, K_RANGE_L, K_RANGE_H) generates a plot showing the trend of the Dice Coefficient and a proxy for the Evidence Lower Bound (ELB/Distortion) across different K-values (e.g., number of clusters). Input Arguments: DICE_COEFFICIENT_FOLDS_ALL - A vector containing the mean Dice Coefficients for each K-value. ELB - A vector containing the corresponding Distortion (or ELBO proxy) values for each K-value. K_RANGE_L - The lowest K-value used in the analysis (for x-axis limit). K_RANGE_H - The highest K-value used in the analysis (
- **Arguments:**
  - `Dice_coefficient_folds_all` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `elb` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `K_range_l` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `K_range_h` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - No explicit return variable; outputs are files, figures, GUI state, console text, or modified structures.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: `whifun_functions/whifun_get_best_k.m:1/whifun_get_best_k`
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.
