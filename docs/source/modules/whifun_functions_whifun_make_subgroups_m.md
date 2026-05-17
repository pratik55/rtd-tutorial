# Module Name: `whifun_functions/whifun_make_subgroups.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.
- **Key Features:**
  - WHIFUN_MAKE_SUBGROUPS Creates minimal overlapping subgroups of subjects from a total pool. [SUBGROUPS, OVERLAPS] = WHIFUN_MAKE_SUBGROUPS(TOTAL_SUBJECTS, N) This function partitions a set of 'total_subjects' into subgroups of size 'n'. If the total number of subjects is not divisible by 'n', the last subgroup is formed by taking the remaining subjects and "filling" the group to size 'n' by randomly sampling subjects from the previously formed full subgroups. This ensures all subgroups are of uniform size 'n', but the last group may overlap with others. Input Arguments: TOTAL_SUBJECTS - The tota
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: No major external dependency pattern detected beyond MATLAB base language.

## Function: `whifun_make_subgroups()`
- **Signature & Definition:** `function [subgroups, overlaps] = whifun_make_subgroups(total_subjects, n)` (line 1)
- **Scientific Theory & Formulas:** Overlap and stability use Dice $D(A,B)=\frac{2|A\cap B|}{|A|+|B|}$ and IoU $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$.
- **Functional Purpose:** WHIFUN_MAKE_SUBGROUPS Creates minimal overlapping subgroups of subjects from a total pool. [SUBGROUPS, OVERLAPS] = WHIFUN_MAKE_SUBGROUPS(TOTAL_SUBJECTS, N) This function partitions a set of 'total_subjects' into subgroups of size 'n'. If the total number of subjects is not divisible by 'n', the last subgroup is formed by taking the remaining subjects and "filling" the group to size 'n' by randomly sampling subjects from the previously formed full subgroups. This ensures all subgroups are of uniform size 'n', but the last group may overlap with others. Input Arguments: TOTAL_SUBJECTS - The total number of subjects available (e.g., number of rows in a data table). N - The desired size of each 
- **Arguments:**
  - `total_subjects` (numeric time-series matrix, commonly T x R, V x T, or T x R x S): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `n` (numeric scalar or numeric vector): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `subgroups` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `overlaps` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.
