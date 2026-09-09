# Longitudinal Behavioral Anomaly Detection for Depression Monitoring Using Passive Smartphone Sensing Data

> Passive smartphone sensing–based longitudinal depression monitoring that combines PHQ-9 severity prediction, individualized behavioral anomaly detection, and lagged temporal analysis.

**Period:** Aug. 2026 - Present  
**Affiliation:** Service Intelligence Laboratory, Ajou University  
**Role:** Undergraduate Research Intern · Sole-author research  
**Status:** Manuscript in preparation  
**Research focus:** Passive sensing · PHQ-9 prediction · Behavioral anomaly detection · Longitudinal / lagged analysis

---

## Overview

This ongoing study uses **BRIGHTEN V1** passive smartphone sensing data and repeated PHQ-9 assessments to model depression as a **participant-level longitudinal process**.

The project has two connected objectives:

1. develop a machine-learning model that predicts **PHQ-9–based depression severity using passive sensing data only**, and
2. detect **individualized behavioral deviations** and test whether those anomalies **precede subsequent PHQ-9 change**.

The central question is whether changes in a participant's everyday behavioral pattern can provide an early signal for longitudinal mental-health monitoring.

![BRIGHTEN dataset overview](assets/figure-01-dataset-overview.webp)

## Research question

> Do individualized behavioral changes observed in passive smartphone sensing occur before subsequent changes in depressive symptoms, and can those deviations be used as meaningful longitudinal monitoring signals?

## Data construction

Passive sensing features and repeated PHQ-9 assessments are aligned at the **participant level** while preserving temporal order.

| Cohort | Participants | Datapoints | Passive features | Follow-up |
|---|---:|---:|---:|---:|
| BRIGHTEN V1 | 541 | 3,007 | 37 | 12 weeks |
| BRIGHTEN V2 | 276 | 1,159 | 111 | 12 weeks |

**Primary analysis:** BRIGHTEN V1  
**Planned reproducibility check:** BRIGHTEN V2

> Participant-level raw data are not redistributed in this repository.

## Analytical framework

![Research objective](assets/figure-02-research-objective.webp)

1. **Longitudinal alignment** — construct participant-level sequences from passive sensing and repeated PHQ-9 assessments.
2. **Depression-severity prediction** — develop a machine-learning model using passive sensing data only.
3. **Personal baseline estimation** — characterize each participant's habitual behavioral pattern.
4. **Behavioral anomaly detection** — identify deviations from the participant-specific baseline.
5. **Lagged temporal analysis** — evaluate whether detected anomalies precede subsequent PHQ-9 change.
6. **Robustness / reproducibility** — compare anomaly definitions and reproduce the analysis when appropriate.

![Sequential representation](assets/figure-03-sequential-representation.webp)

## Current status

This is an ongoing study, so this repository does **not** present a final predictive-performance claim yet. Current work focuses on participant heterogeneity, missingness, sequence construction, prediction modeling, individualized anomaly definitions, and temporal validation.

## Why this matters

Population-level prediction can identify average risk but may fail to capture clinically meaningful **within-person change**. This project therefore shifts the unit of interpretation from only between-person differences toward **deviation from an individual's own behavioral history**.

The intended direction is a personalized monitoring framework that connects:

**passive sensing → depression-severity prediction → individualized behavioral anomaly → subsequent symptom change**.

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

- [`outputs/methodology-seminar-public-excerpt.pdf`](outputs/methodology-seminar-public-excerpt.pdf) — public-safe excerpt documenting the dataset framing and sequence-preserving analysis direction.
- [`outputs/PROJECT_OUTPUTS.md`](outputs/PROJECT_OUTPUTS.md) — provenance, scope, and release notes for public artifacts.

## Repository scope

This repository documents the **research framing, analytical design, selected source-derived figures, and public-safe outputs**. Original BRIGHTEN participant-level data are not included, and analysis code will only be released when compatible with dataset-use restrictions and a stabilized analysis interface.

---

**Junha Won**  
Ajou University · Department of Industrial Engineering  
[Portfolio detail](https://juna0926.github.io/Portfolio/research/brighten.html) · [Portfolio](https://juna0926.github.io/Portfolio/) · [GitHub](https://github.com/Juna0926)
