# Module Name: `whifun_functions/fd_calc.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Key Features:**
  - FD_CALC Calculates the Framewise Displacement (FD) from a time series of rigid-body head motion parameters. FD = FD_CALC(Y) Framewise Displacement is a scalar quantity summarizing head motion from one time point to the next, typically derived from 6 rigid-body realignment parameters (3 translations and 3 rotations). Rotations are usually converted to displacements on a sphere of a given radius (e.g., 50 mm). Input Arguments: Y - Head motion parameters time series. Expected size: N_TimePoints x N_MotionParameters (where N_MotionParameters is 6, or 12 if including derivatives, but only the 6 pri
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `fd_calc()`
- **Signature & Definition:** `function fd = fd_calc(Y)` (line 1)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Spherical ROI selection uses $d=\sqrt{\sum_a(\Delta v_a s_a)^2}\le r$ and affine MNI-voxel transforms.
- **Functional Purpose:** FD_CALC Calculates the Framewise Displacement (FD) from a time series of rigid-body head motion parameters. FD = FD_CALC(Y) Framewise Displacement is a scalar quantity summarizing head motion from one time point to the next, typically derived from 6 rigid-body realignment parameters (3 translations and 3 rotations). Rotations are usually converted to displacements on a sphere of a given radius (e.g., 50 mm). Input Arguments: Y - Head motion parameters time series. Expected size: N_TimePoints x N_MotionParameters (where N_MotionParameters is 6, or 12 if including derivatives, but only the 6 primary parameters are used for FD calculation, typically after rotational parameters have been convert
- **Arguments:**
  - `Y` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `fd` (numeric scalar or numeric vector): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** No explicit defensive branch was detected; incompatible inputs will fail through MATLAB runtime behavior.
