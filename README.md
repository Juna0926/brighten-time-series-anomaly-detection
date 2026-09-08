# Longitudinal Behavioral Anomaly Detection for Depression Monitoring Using Passive Smartphone Sensing Data

> Longitudinal digital-health research using passive smartphone sensing to predict PHQ-9–based depression severity and test whether individualized behavioral anomalies precede subsequent symptom change.

**Period:** Aug. 2026 - Present  
**Affiliation:** Service Intelligence Laboratory, Ajou University  
**Role:** Undergraduate Research Intern · Independent research project  
**Status:** Sole-author manuscript in preparation  
**Research focus:** Passive sensing · PHQ-9 prediction · Behavioral anomaly detection · Lagged temporal analysis

---

## Overview

This study uses **BRIGHTEN V1** passive smartphone sensing data and repeated PHQ-9 assessments to model depression as a **participant-level longitudinal process**. The current work has two connected goals:

1. predict PHQ-9–based depression severity using **passive sensing data only**, and
2. detect individualized behavioral deviations and evaluate whether they **precede subsequent PHQ-9 change**.

The study therefore moves beyond a population-only risk model and asks whether changes relative to a participant's own behavioral history can provide a useful signal for longitudinal mental-health monitoring.

![BRIGHTEN dataset overview](assets/figure-01-dataset-overview.webp)

## Research questions

- Can passive smartphone sensing alone predict PHQ-9–based depression severity?
- Can a participant-specific behavioral baseline be used to identify meaningful behavioral anomalies?
- Do detected anomalies occur before subsequent changes in PHQ-9 scores?

## Data construction

Passive sensing features and repeated PHQ-9 assessments are aligned at the participant level so that temporal ordering is preserved.

| Cohort | Participants | Datapoints | Passive features | Follow-up |
|---|---:|---:|---:|---:|
| BRIGHTEN V1 | 541 | 3,007 | 37 | 12 weeks |
| BRIGHTEN V2 | 276 | 1,159 | 111 | 12 weeks |

**Primary analysis:** BRIGHTEN V1  
**Planned reproducibility check:** BRIGHTEN V2

> Participant-level raw data are not redistributed in this repository.

## Analytical framework

![Research objective](assets/figure-02-research-objective.webp)

1. **Longitudinal alignment** - construct participant-level sequences from passive sensing and repeated PHQ-9 assessments.
2. **Depression-severity prediction** - develop a machine-learning model using passive sensing data only.
3. **Personal baseline estimation** - characterize each participant's habitual behavioral pattern.
4. **Behavioral anomaly detection** - identify deviations from the participant-specific baseline.
5. **Lagged temporal analysis** - test whether detected anomalies precede subsequent PHQ-9 change.
6. **Robustness / replication** - evaluate alternative anomaly definitions and reproduce the analysis when appropriate.

![Sequential representation](assets/figure-03-sequential-representation.webp)

## Current status

This is an ongoing study. The repository does **not** report a final predictive-performance claim yet. Current work focuses on participant heterogeneity, missingness, sequence construction, prediction modeling, anomaly definitions, and temporal validation.

## Why this matters

A single population-level prediction can identify average risk but may miss clinically meaningful **within-person change**. This project explores a personalized monitoring framework that combines passive sensing, depression-severity prediction, and individualized behavioral deviation to detect changes that may occur before worsening self-reported symptoms.

## My contribution

- Research-question and analytical-framework design
- Participant-level longitudinal dataset construction
- Passive-sensing feature analysis
- PHQ-9 severity prediction modeling
- Individualized behavioral-anomaly design
- Lagged temporal analysis with subsequent PHQ-9 change
- Reproducibility design using BRIGHTEN V2
- Visualization and manuscript preparation

## Public outputs

- [`outputs/methodology-seminar-public-excerpt.pdf`](outputs/methodology-seminar-public-excerpt.pdf) - public-safe excerpt documenting the dataset framing and sequence-preserving analysis direction.
- [`outputs/PROJECT_OUTPUTS.md`](outputs/PROJECT_OUTPUTS.md) - provenance, scope, and release notes for public artifacts.
- Original BRIGHTEN participant-level data are not included.

## Repository scope

This is a **research portfolio repository**. It documents the study design, selected source-derived figures, and public-safe artifacts. Analysis code will only be published when release is compatible with dataset-use restrictions and the analysis interface is stabilized.

---

**Junha Won**  
Ajou University, Department of Industrial Engineering  
[Portfolio detail](https://juna0926.github.io/Portfolio/research/brighten.html) · [Portfolio](https://juna0926.github.io/Portfolio/) · [GitHub](https://github.com/Juna0926)
