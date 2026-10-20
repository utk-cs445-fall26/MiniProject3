# Disagreement Review — smazunda

**Project owner:** `ggood3`  
**Validator:** `smazunda`  

This document summarizes the nine records marked `No` in `smazunda_validation_log.csv` (1 `Currentstatus` and 8 `RecentThemes`). Each was discussed using the commit evidence and the coding guide, and an adjudicated value was decided and noted down. Please find the same in `smazunda_disagreement_resolution.csv` or from line 31 within this document.

## Three distinct disagreement examples and resolutions

### 1. `smistad_fast` — `Currentstatus`
- **Author value:** `Needs verification`
- **Validator value:** `Active`
- **Key evidence:** Latest commit on or before 2025-09-30 in the supplied summary is 2025-09-29, after 2025-04-01; codebook cutoff gives Active.
- **Discussion outcome:** Latest commit in the supplied summary is 2025-09-29, after the 2025-04-01 cutoff in the coding guide, so the rule gives Active. 'Needs verification' was not needed once the date was checked.
- **Adjudicated value / Resolution type / Post-discussion agreement:** `Active` / Validator Kept / `Yes`

### 2. `vida-nyu_reprozip` — `RecentThemes`
- **Author value:** `Other:Dependency updates`
- **Validator value:** `Release and Documentation updates`
- **Key evidence:** Latest 10 available commits include version bumps, Python 2 compatibility removal, security.txt and .nojekyll files, and merge commits; strongest themes are Release and Documentation updates.
- **Discussion outcome:** Recent commits are version bumps, Python 2 removal and security.txt/.nojekyll files. Wwe decided that dependency updates was not dominant, so we narrowed the label to Release Updates, considering documentation files as secondary.
- **Adjudicated value / Resolution type / Post-discussion agreement:** `Release Updates` / Compromise / `Yes`

### 3. `llnl_mgmol` — `RecentThemes`
- **Author value:** `Bug fixes:Other`
- **Validator value:** `Bug fixes and Feature development`
- **Key evidence:** Recent available messages include fixes to generated file headers, stdout, compiler warnings, and new/extended functionality; strongest themes are Bug fixes and Feature development.
- **Discussion outcome:** Recent messages consisted of header/stdout/compiler warning fixes. Since both labels contained Bug fixes, final decision was to keep the theme.
- **Adjudicated value / Resolution type / Post-discussion agreement:** `Bug fixes` / Compromise / `Yes`

## Summary of all resolved disagreements

| Project ID | Field | Author value | Validator value | Adjudicated value | Resolution type | Post-discuss agreement |
|---|---|---|---|---|---|---|
| smistad_fast | Currentstatus | Needs verification | Active | Active | Validator Kept | Yes |
| vida-nyu_reprozip | RecentThemes | Other:Dependency updates | Release and Documentation updates | Release Updates | Compromise | Yes |
| llnl_mgmol | RecentThemes | Bug fixes:Other | Bug fixes and Feature development | Bug fixes | Compromise | Yes |
| smistad_fast | RecentThemes | Other:Feature development | Feature development and Bug fixes | Feature Development | Compromise | Yes |
| mouseland_kilosort | RecentThemes | Other:Bug fixes | Bug fixes and Documentation updates | Bug and Documentation updates | Validator Kept | Yes |
| martini-alessandro_maximum-entropy-spectrum | RecentThemes | Documentation updates | Documentation updates and Other (research-paper revisions) | Documentation Updates | Author Kept | Yes |
| shixiangwang_sigminer | RecentThemes | Automated bot contributions:Other | Bug fixes and Documentation updates | Automated Document Contributions | Compromise | Yes |
| worldwidetelescope_wwt-website | RecentThemes | Other:Automated bot contributions | Dependency updates and Bug fixes | Automated Dependency Contributions | Compromise | Yes |
| natverse_nat.nblast | RecentThemes | Automated bot contributions:Documentation updates | Release and Dependency updates | Documentation Updates | Author Kept | Yes |

## Follow-up status

All nine disagreements have an adjudicated value, a resolution type and a post-discussion agreement of `Yes`. Resolution types: 2 Validator Kept, 2 Author Kept and 5 Compromise. These are recorded in `smazunda_disagreement_resolution.csv`, and the post-discussion figures are in `smazunda_agreement_stats.csv`.
