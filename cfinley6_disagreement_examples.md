# MiniProject 3 Part 2: Disagreement Examples & Qualitative Adjudication

**Parties of Discussion:**
* **Project Owner / Author:** Alex Rother (`arother1`)
* **Validator:** Connor Finley (`cfinley6`)

---

## Overview
Following the independent validation review of 10 open-source software projects in Part 1, we held an evidence-based adjudication meeting to review records where discrepancies existed between author and validator values. Below are 3 distinct examples documenting the nature of the disagreement, the evidence evaluated, and the final adjudicated resolution.

---

## Example 1: `ssl-hep_servicex` — Field: `ActivityPattern`

* **Project ID:** `ssl-hep_servicex`
* **Parties:** `arother1` (Project Owner) & `cfinley6` (Validator)
* **Initial Author Value:** `declining`
* **Initial Validator Value:** `irregular`
* **Pre-Discussion Agreement Status:** `No`

### Evidence Evaluated
* **Commit History:** The project sees activity in almost every observed month, but volume has dropped significantly from its early high-volume years. 
* **Recent Commits:** Recent activity shows micro-bursts of Dependabot updates rather than a smooth downward curve.

### Discussion & Resolution
`cfinley6` initially marked the pattern as `irregular` because the remaining commits appeared in sporadic bursts rather than a perfectly smooth decline. `arother1` pointed out that looking at the macro year-over-year trend, the overall volume definitively and permanently shifted downward, which fits the `declining` archetype better than a baseline of random chaos. The validator yielded to the macro trend.

* **Adjudicated Value:** `declining`
* **Resolution Type:** `AuthorKept`
* **Post-Discussion Agreement Status:** `Yes`

---

## Example 2: `genetics-statistics_gemma` — Field: `RecentThemes`

* **Project ID:** `genetics-statistics_gemma`
* **Parties:** `arother1` (Project Owner) & `cfinley6` (Validator)
* **Initial Author Value:** `Documentation updates:Feature development`
* **Initial Validator Value:** `Documentation updates:Bug fixes`
* **Pre-Discussion Agreement Status:** `No`

### Evidence Evaluated
* **Recent Commits (Post-Gap):** Commits `f112b0fa5`, `8c82a8294`, and `7c4f7f7f7` explicitly repair broken GCC 10 builds, and commit `57b3a882c` fixes failing test suites.

### Discussion & Resolution
`arother1` categorized the return activity as "Feature development" alongside documentation. `cfinley6` argued that repairing a build pipeline for a new compiler version (GCC 10) and fixing failing tests falls strictly under "Bug fixes" (maintenance and toolchain compatibility) rather than net-new product features. `arother1` reviewed the commit hashes and agreed with the reclassification.

* **Adjudicated Value:** `Documentation updates:Bug fixes`
* **Resolution Type:** `ValidatorKept`
* **Post-Discussion Agreement Status:** `Yes`

---

## Example 3: `semanticchemistry_semanticchemistry` — Field: `Currentstatus`

* **Project ID:** `semanticchemistry_semanticchemistry`
* **Parties:** `arother1` (Project Owner) & `cfinley6` (Validator)
* **Initial Author Value:** `Inactive`
* **Initial Validator Value:** `Active`
* **Pre-Discussion Agreement Status:** `No`

### Evidence Evaluated
* **GitHub Repository Status:** The repository has visible commits in January 2026.
* **Rubric Constraints:** Data cutoff date for this assignment was strictly defined as `2025-09-30`.

### Discussion & Resolution
`cfinley6` saw the January 2026 commits on GitHub and labeled the project as `Active`. `arother1` pointed out that as of the strict course cutoff date (September 30, 2025), the project had been dormant for an extended period, meaning its historical status relative to the dataset was technically `Inactive`. `cfinley6` agreed to adhere strictly to the temporal bounds of the assignment dataset.

* **Adjudicated Value:** `Inactive`
* **Resolution Type:** `AuthorKept`
* **Post-Discussion Agreement Status:** `Yes`
