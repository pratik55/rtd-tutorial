# Module Name: `whifun_functions/fdr_bh.m`
- **Module Category:** WhiFuN first-party MATLAB function.
- **Theoretical Background:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Benjamini-Hochberg FDR retains sorted $p_{(i)}\le iq/m$; Bonferroni uses $\alpha/m$.
- **Key Features:**
  - fdr_bh() - Executes the Benjamini & Hochberg (1995) and the Benjamini & Yekutieli (2001) procedure for controlling the false discovery rate (FDR) of a family of hypothesis tests. FDR is the expected proportion of rejected hypotheses that are mistakenly rejected (i.e., the null hypothesis is actually true for those tests). FDR is a somewhat less conservative/more powerful method for correcting for multiple comparisons than procedures like Bonferroni correction that provide strong control of the family-wise error rate (i.e., the probability that one or more null hypotheses are mistakenly rejecte
  - Internal calls detected: No internal WhiFuN calls detected.
  - External dependencies detected: Statistics and Machine Learning Toolbox

## Function: `fdr_bh()`
- **Signature & Definition:** `function [h, crit_p, adj_ci_cvrg, adj_p]=fdr_bh(pvals,q,method,report)` (line 131)
- **Scientific Theory & Formulas:** Framewise displacement is commonly $FD_t=\sum_{i=1}^{3}|\Delta d_{i,t}|+R\sum_{i=1}^{3}|\Delta\theta_{i,t}|$, with $R=50\,\mathrm{mm}$. Benjamini-Hochberg FDR retains sorted $p_{(i)}\le iq/m$; Bonferroni uses $\alpha/m$.
- **Functional Purpose:** fdr_bh() - Executes the Benjamini & Hochberg (1995) and the Benjamini & Yekutieli (2001) procedure for controlling the false discovery rate (FDR) of a family of hypothesis tests. FDR is the expected proportion of rejected hypotheses that are mistakenly rejected (i.e., the null hypothesis is actually true for those tests). FDR is a somewhat less conservative/more powerful method for correcting for multiple comparisons than procedures like Bonferroni correction that provide strong control of the family-wise error rate (i.e., the probability that one or more null hypotheses are mistakenly rejecte
- **Arguments:**
  - `pvals` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `q` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `method` (character vector, string scalar, or categorical option): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
  - `report` (MATLAB value inferred from source usage): Inferred from the signature, variable name, and source usage; precise validation occurs at MATLAB runtime.
- **Returns:**
  - `h` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `crit_p` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `adj_ci_cvrg` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
  - `adj_p` (MATLAB value inferred from source usage): Output produced by the MATLAB implementation.
- **Dependencies:**
  - Calls: No internal WhiFuN calls detected in this function body.
  - External: No major external dependency pattern detected beyond MATLAB base language.
  - Called By: No internal caller detected by static scan; entry point, callback, script-local function, or externally invoked routine.
- **Edge Cases & Exceptions:** Defines defaults or branches for optional arguments or missing files. Checks empty arrays, missing files, or empty user selections. Raises MATLAB errors for invalid dimensions, missing files, invalid parameters, or failed commands.
