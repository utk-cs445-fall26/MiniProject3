# Disagreements for hsaleh5

Author: Jacob Yuill (`jtyuill`). Validator: Hamzah Saleh (`hsaleh5`). These are the parties for every example below. There were 11 disagreements out of 50 comparisons. Jacob accepted all 11 proposed validator changes by message. All 11 are recorded as ValidatorKept with post-discussion agreement Yes. The other 39 labels were retained.

I reviewed Jacob's [MiniProject2 snapshot](https://github.com/jtyuill/MiniProject2/tree/9db1f2e88ffa2b28ff366a4a2e0d69c3fe71a394), including its stats, commit messages, gap records, monthly series, plots and reflections. Filenames and commit hashes in the validation log refer to that snapshot. The latest ten records are sorted by timestamp, with SHA as the tie breaker. This keeps the review repeatable instead of mixing saved WoC data with newer GitHub commits. WoC includes contributor branches and PR merge records, so a record is not automatically an upstream release or merged feature.

For themes, I used the referenced source message when a merge message supplied its SHA. A commit can support two themes, such as a bot dependency update or a documentation bug fix. Theme order does not affect agreement. Ties use the order in the coding guide. Formatting, generic integration and compiler-portability work are Other unless a more specific theme is clear. For Currentstatus, I checked upstream default-branch history through September 30, 2025. I treated resumed bot or documentation commits as recovery because the guide does not require a feature release or a three-month gap.

## 1. CascadeStudio: Currentstatus

Project: `zalo_cascadestudio`.

- Author value: Active.
- Validator value: Inactive.
- Evidence: The last upstream default-branch commit by the cutoff was [c022498e67 on January 2, 2025](https://github.com/zalo/CascadeStudio/commit/c022498e67a2574e532aecc3f287900de66cb277). The saved WoC data contains additional bot/PR merge records through March 14, 2025. Both dates are before April 1, 2025, so the project is Inactive under the guide. The author's lastGHCommitDate is in June 2026, which answers a different time window.
- Resolution: ValidatorKept, Inactive. Jacob accepted this correction as part of his acceptance of all 11 changes.

## 2. TensorFlow.js: HasRecovered and WhyRecovered

Project: `tensorflow_tfjs`.

- Author values: HasRecovered = N/A; WhyRecovered = N/A no gap of 3+ months.
- Validator values: HasRecovered = Yes; WhyRecovered = Dependabot dependency updates resumed in November 2025 after the one empty month. This is maintenance activity, not evidence of a feature revival.
- Evidence: The monthly series has no commits in October 2025. The gap records then show a Dependabot update on November 13 (`db6ea6ae51`) and another on November 16 (`b40205bd7b`). The guide asks whether activity resumed after the longest gap. It does not set a three-month minimum and lists new commits as evidence.
- Resolution: ValidatorKept for both fields. Count the return of maintenance activity without claiming that feature development recovered. Jacob accepted both changes.

## 3. CascadeStudio: WhyRecovered

Project: `zalo_cascadestudio`.

- Author value: zalo came back in 2026 and rewrote a lot of it as CascadeStudio v2.
- Validator value: A contributor updated the README link in October 2024, and the maintainer merged that change in January 2025. This ended the recorded gap through documentation maintenance.
- Evidence: The gap runs from August 2023 through September 2024. Pasukhin Dmitry's October 10, 2024 README change is `b922479d13`, and its January 2, 2025 merge is `c022498e67`. These records end the saved gap before the claimed 2026 rewrite. The later comeback and the first activity after the gap should be described separately.
- Resolution: ValidatorKept. Keep HasRecovered = Yes, but explain the first restart as documentation maintenance. Jacob accepted this explanation.

## 4. RecentThemes: use the same ten commits

These seven disagreements all use the saved snapshot's latest ten records. Detailed dates and hashes are in `hsaleh5_validation_log.csv`.

| Project | Author value | Validator value | Evidence |
| --- | --- | --- | --- |
| `ifcopenshell_ifcopenshell` | Dependency updates:Release | Feature development:Bug fixes | November 2025 records add profiler/UI/search features and fix drawing behavior. There is no release commit in this window. |
| `lastools_lastools` | Release:Documentation updates | Bug fixes:Other | August-October 2025 records fix builds, CMake and memory errors, and add compiler portability. There is no release or README update in the window. |
| `opendatacube_datacube-explorer` | Dependency updates:Automated bot contributions | Bug fixes:Automated bot contributions | Four documentation-build/test fixes and three bot-related records appear among the ten. The fixes should be represented. |
| `choderalab_pymbar` | Bug fixes:Feature development | Other:Bug fixes | February 2026 records include five vague-update/lint/integration records, three test/tolerance-fix records, and two feature records. Other is common in this particular window. |
| `tensorflow_tfjs` | Other:Bug fixes | Dependency updates:Automated bot contributions | All ten April 14-17, 2026 records are Dependabot dependency bumps or their matching merges, including follow-redirects and protobufjs. |
| `zalo_cascadestudio` | Release:Security patches | Dependency updates:Automated bot contributions | Seven of the ten saved records are bot dependency updates or matching merges. The other three concern the README. No release appears in this window. |
| `johannfaouzi_pyts` | Dependency updates:Release | Bug fixes:Documentation updates | June 2025 records fix deprecated APIs, examples and documentation. One dependency constraint change appears, but no release commit does. |

Resolution for each row: ValidatorKept, using the validator's two themes as the adjudicated value. Jacob accepted all seven theme changes. Some messages still allow more than one interpretation, but these are the agreed labels for the shared review window.

## Agreement results

Pre-discussion agreement is 90.0% for HasRecovered, 80.0% for WhyRecovered, 100.0% for ActivityPattern, 90.0% for Currentstatus and 30.0% for RecentThemes. That is 39 agreements out of 50 comparisons overall. Prose values with the same supported meaning were retained rather than counted as wording disagreements.

Kappa uses the two raters' observed category frequencies. HasRecovered has pre-discussion kappa 0.0000 because the validator assigned Yes to every project while the author assigned nine Yes values and one N/A. The author's N/A is retained as a recorded category for this calculation. ActivityPattern has pre-discussion kappa 1.0000 and Currentstatus has pre-discussion kappa 0.6154. The two non-categorical fields use NA.

After Jacob's acceptance, all five fields have 100.0% agreement. All 11 disagreements are resolved. Post-discussion kappa is 1.0000 for ActivityPattern and Currentstatus. HasRecovered uses NA because both final rating vectors contain only Yes, making expected agreement equal to 1 and kappa undefined. Post-discussion agreement measures the accepted consensus, not a second independent coding exercise.

Jacob's separate 50-row validation log of Hamzah's ten projects is included as `jtyuill_validation_log.csv`. Hamzah accepted all ten of Jacob's proposed changes. Its adjudicated values are filled, and each changed row records ValidatorKept with post-discussion agreement Yes in Comments. The two logs now contain 100 finalized comparisons, with 21 disagreements resolved in total. The five rows in `hsaleh5_agreement_stats.csv` summarize Hamzah's review of Jacob's ten projects only, using ten comparisons per field.


## Reciprocal review: Jacob's corrections to Hamzah's projects

Author: Hamzah Saleh (`hsaleh5`). Validator: Jacob Yuill (`jtyuill`). Hamzah accepted all ten changes below. Each resolution is ValidatorKept, and post-discussion agreement is Yes. Original author and validator values and the full evidence are preserved in `jtyuill_validation_log.csv`.

| Project | Field | Adjudicated value | Evidence and resolution reason |
| --- | --- | --- | --- |
| `vibansal_hapcut2` | HasRecovered | No | One isolated maintainer CRAM-parsing commit followed the long gap; other saved records include unmerged PR work. Accepted Jacob's distinction between an isolated change and sustained recovery. |
| `vibansal_hapcut2` | WhyRecovered | No real recovery; isolated maintainer feature commit (CRAM parsing, 2025-02-09) plus unmerged outside PR #137 (Makefile) | The CRAM change is `9a10aba2a6`; PR #137 was still unmerged in the reviewed evidence. |
| `friendly_heplots` | ActivityPattern | irregular | The full series alternates bursts and long gaps. Recent high activity alone does not establish a sustained rise across the entire history. |
| `neuroml_neuroml2` | ActivityPattern | declining | Activity fell after the 2021 peak, and the series did not end with sustained recovery. |
| `modelica_modelica_linearsystems2` | ActivityPattern | irregular | Development appears in separated bursts, including 2012, 2017, 2020-2021 and 2024. |
| `lsstdesc_ccl` | ActivityPattern | irregular | The 2023 increase interrupts the proposed gradual decline. The recent slowdown is real, but does not describe the whole history. |
| `dsavransky_exosims` | ActivityPattern | declining | Annual totals taper after the 2018 peak rather than varying without a trend. |
| `vibansal_hapcut2` | RecentThemes | Bug fixes:Documentation updates | Build/gcc fixes outnumber feature changes in the reviewed ten-commit window. |
| `elki-project_elki` | RecentThemes | Feature development:Bug fixes | Algorithm/data-structure additions and error fixes outweigh cleanup work. |
| `modelica_modelica_linearsystems2` | RecentThemes | Bug fixes:Documentation updates | Empty-state-matrix and printing fixes change behavior; they should not all be coded Other. |

The HapCUT2 decision leaves a definition issue worth documenting: Jacob judged sustained recovery, while the first review counted resumed maintenance after a gap. Both accepted interpretations are recorded explicitly. A future codebook should distinguish any resumed activity from a sustained return so these labels are more consistent.
