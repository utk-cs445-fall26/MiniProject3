# Validation Reflection — smazunda

## Agreement results

`HasRecovered` and `ActivityPattern` each had 10 of 10 records in agreement, and `Currentstatus` had 9 of 10 (Cohen's k  = 0.75 before discussion). `WhyRecovered` also agreed on 10 of 10 records, although this is a free-text field which was judged on substance rather than wording. The largest source of disagreement was `RecentThemes`, with only 2 of 10 records in agreement. After the nine disagreements were adjudicated with project owner `ggood3`, post-discussion agreement was 100.0% for all five fields, and Cohen's k for `Currentstatus` rose to 1.0. `HasRecovered` has Cohen's k = NA because every label is "Yes". Please find the figures in `smazunda_agreement_stats.csv`, and the resolutions in `smazunda_disagreement_resolution.csv` and `smazunda_disagreement.md`.

## Early signs of long gaps

The records show few warning signs inside the commit messages themselves, and looks like the clearest signals come from the activity-pattern labels. Four of the ten projects (`vida-nyu_reprozip`, `smistad_fast`, `shixiangwang_sigminer`, `natverse_nat.nblast`) are labelled declining, which means their overall commit volume was already falling before their gaps. While, two (`llnl_mgmol`, `q2mm_q2mm`) are U-shaped, a long gap followed by renewed commits, and three (`scifio_scifio-imageio`, `martini-alessandro_maximum-entropy-spectrum`, `worldwidetelescope_wwt-website`) are irregular, with uneven bursts with Only `mouseland_kilosort` being labelled rising. The gaps themselves vary in length, which can be said are roughly ten months for `vida-nyu_reprozip` (2025-02 to 2025-11), about ten months for `llnl_mgmol` (2022-03 to 2023-01), and about two years for `scifio_scifio-imageio` (2022-06 to 2024-05). Finally, a decline in volume, a small burst of release, then silence was the most common shape.

## What triggers recovery

In every reviewed project, activity resumed with release work rather than a large redesign. Examples include the 1.3.1 and 1.3.2 releases and removal of Python 2 support in `vida-nyu_reprozip`, mixed build fixes in `llnl_mgmol`, and a CI upgrade for ITK 5.4.0 in `scifio_scifio-imageio`. Other projects looked like they restarted with bug fixes, dependency and environment changes, or documentation updates. The commit records show what work resumed, but they do not establish the reasons for the earlier gap, and the labels avoid claiming the same.

## When a gap does not mean the project is dead

All ten projects were marked `HasRecovered = Yes`, because commits resumed after the longest gap, just like how `vida-nyu_reprozip` and `martini-alessandro_maximum-entropy-spectrum` are `Currentstatus = Inactive` under the 2025-04-01 cutoff (last commits 2025-01-27 and 2024-11-18 in the supplied summary), yet `vida-nyu_reprozip` shows commits resuming in December 2025. `Currentstatus` can be said was against a fixed rule and cutoff date, while `HasRecovered` looks at the full history. Both labels can be correct at the same time, and the dates had to be checked before concluding that a project is abandoned.

## Interpretation pitfalls and how they were resolved

1. **Classifying mixed commit sets** The 8 `RecentThemes` disagreements mostly came from commit sets that had dependency updates, release documentation, bug fixes and features. One reviewer chose `Other` or automated bot contributions, while the other chose the technical purpose of the changes. On discussing, we decided to separate the dominant theme from routine concepts like merge commits, version bumps and bot-generated pull requests. Five of the nine resolutions were compromises, which shows how often the two labels were significantly close.
2. **Reading too much into one signal** One recent burst of activity should not change a long-term `ActivityPattern` label and hence the full time series matters.
3. **Applying the cutoff rule** The `smistad_fast` `Currentstatus` disagreement ("Needs verification" vs "Active") was resolved by applying the coding guide's cutoff to the dated commit, which gave Active.
4. **Inferring more than the evidence supports** A returning commit shows what work resumed but usually cannot prove why the project was inactive. Keeping `WhyRecovered` descriptions tied to noticed commits kept the labels consistent among reviewers.
5. **Limits of the evidence** The `RecentThemes` validations rely on the latest available commit messages in the supplied summary, so we can treat them as tentative if the export may be incomplete.
