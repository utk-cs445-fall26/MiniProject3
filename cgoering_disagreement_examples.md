# MiniProject3 - Disagreement Examples

Parties: Camden Goering (`cgoering`) and Davyn Mengeling (`dmengeli`). We resolved all 34 pre-discussion disagreements (22 on my projects, 12 on his) over text. Full list: `cgoering_disagreement_resolution.csv`.

## Example 1: Is one trivial commit a "recovery"? (HasRecovered)

- **Projects:** `exascaleinfolab_vadetis` (owner cgoering, validator dmengeli) and `ashiklom_edr-da` (owner dmengeli, validator cgoering)
- **Values before discussion:** I had vadetis as `Yes`; Davyn had `No`. Davyn had ashiklom as `Yes`; I had `No`.
- **Evidence:** vadetis had a 41-month gap (2021-08 to 2024-12) and only two commits after it, both "Update README.md" on 2025-01-03. ashiklom had a 49-month gap and one post-gap commit, "Create LICENSE" (2025-06-20). `svalorzen_ai-toolbox` (3 post-gap commits, mostly CI and automatic merges) and `pseudomanifold_aleph` (one "Fixed PKGBUILD url" commit after 29 months) fit the same pattern.
- **Resolution:** `No` for all four (ValidatorKept on my projects, ValidatorKept on his). We agreed on one standard: new commits after a gap do not count as recovery unless they show sustained development.

## Example 2: Contradicting the author's own dates (Currentstatus)

- **Projects:** `lampspuc_statespacemodels.jl` and `trichter_rf` (owner dmengeli, validator cgoering)
- **Values before discussion:** Davyn had `Inactive` for both; I had `Active`.
- **Evidence:** the coding guide marks a project Inactive only if its last commit is before 2025-04-01. Davyn's own stats file lists last GitHub commits of 2026-08-24 (lampspuc) and 2026-05-05 (trichter_rf), and the World of Code data ends 2026-03-19 and 2026-02-24.
- **Resolution:** `Active` for both (ValidatorKept). Davyn agreed.

## Example 3: Counting automatic merge commits (RecentThemes)

- **Projects:** `facebookresearch_faiss` and `sasview_sasview` (owner cgoering, validator dmengeli)
- **Values before discussion:** For faiss I had `Feature development:Documentation updates` and Davyn had `Other:Dependency updates`. For sasview I had `Feature development:Documentation updates` and Davyn had `Other:Dependency updates`.
- **Evidence:** 9 of faiss's last 10 commits are automatic "Merge <sha> into <sha>" commits, plus one "Update API docs". All but one of sasview's last 10 are the same kind of merge, and the one real PR is named "doc-locating". Neither project's last 10 shows dependency work or feature work.
- **Resolution:** `Other:Documentation updates` for both (Compromise). Davyn's "Other" for the merge commits was right, my documentation label was right, and the other two labels had no support in the commits.

## Example 4: My unedited placeholders (WhyRecovered)

- **Projects:** all ten of mine, e.g. `gems-uff_noworkflow` (owner cgoering, validator dmengeli)
- **Values before discussion:** my value was auto-draft text ("DRAFT - after gap commits are mostly ... Feature development"); Davyn wrote "Development resumed with database import features and follow-up fixes."
- **Evidence:** the first commits after the gap were "Add command to import content database" and relational import work.
- **Resolution:** Davyn's wording (ValidatorKept) for all ten; the `N/A - not recovered` form for vadetis and ai-toolbox following Example 1.
