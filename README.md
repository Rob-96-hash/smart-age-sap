# Statistical Analysis Plan — Weather and Walking Time in Older Adults (SMART-AGE)

This repository holds the versioned Statistical Analysis Plan (SAP) for a master's
thesis on ambient weather and accelerometer-derived walking time in
community-dwelling older adults, based on the SMART-AGE cohort (Heidelberg).

The plan was written before the analysis and amended during the project. Every
version is kept here so that the sequence of decisions, and the point at which
each was fixed, can be checked against the reported results.

**Author:** Robert Seidel, University of Konstanz, Social and Economic Data Science

## Study in brief

Accelerometer-derived walking time was analysed for 245 community-dwelling older
adults observed in two waves. A Tweedie generalized additive mixed model with a
Mundlak decomposition separates within-person from between-person weather
exposure, at two aggregation levels (four-hour day phases and full waking days).
Weather is assigned at district level from 20 local stations.

## Versions

| Version | Date | Change |
|:---|:---|:---|
| 1.0 | 06.02.2026 | Original version (first draft) |
| 1.1 | 09.04.2026 | Updated version |
| 1.2 | 13.05.2026 | Correction of design |
| 1.3 | 13.05.2026 | Within-person effects introduced as the primary target, reporting of EDF, definition of effect ranges |
| 1.4 | 20.05.2026 | H3 deleted, counterfactual analysis on observed percentiles introduced, robustness checks added |
| 1.5 | 18.06.2026 | Between-person terms changed from linear to smooth, wave-season rule extended from temperature to all weather variables |
| 1.6 | 24.06.2026 | Between-person terms returned to linear (original Mundlak specification), statistical power at the person level, GPBoost tuning |
| 1.7 | 01.08.2026 | Humidex introduced, person-cluster bootstrap, covariate robustness specified on gait speed |
| 1.8 | 12.08.2026 | Adjusted predictions, all models estimated on complete cases for comparability |

Versions 1.0 to 1.2 are documented in the amendment history of the later files
but are not included as separate documents.

## Files

Each file is the signed SAP main text for that version. `SAP_v1.8.docx` is the
current one. The amendment history inside each document lists the changes
relative to its predecessor.

## Scope

This repository contains the analysis plan only. It holds no participant data.
The cohort data are not publicly available.
