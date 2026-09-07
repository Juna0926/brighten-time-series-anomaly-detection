# BRIGHTEN Time-Series Behavioral Anomaly Detection

> Personalized depression monitoring from passive smartphone sensing, with PHQ-9 as the clinical outcome and within-person behavioral change as the central signal.

**Period:** Aug. 2026 - Present  
**Affiliation:** Service Intelligence Laboratory, Ajou University  
**Role:** Undergraduate Researcher / Independent research project  
**Status:** Ongoing research; sole-author manuscript in preparation

---

## Overview

This study asks whether changes in a person's passive smartphone-sensing pattern can provide an earlier signal of subsequent change in depressive symptoms. The analysis is intentionally framed as a **within-person time-series problem** rather than a population-only classification problem.

The current study uses **PHQ-9 as the primary outcome**. Passive sensing variables are organized as participant-level daily sequences so that temporal order is preserved instead of reducing each week to a single average feature vector.

![BRIGHTEN dataset overview](assets/figure-01-dataset-overview.png)

## Research question

**Do individualized behavioral anomalies in passive smartphone sensing precede subsequent PHQ-9 change?**

The analytical target is a meaningful deviation from each participant's own habitual behavioral baseline. This supports the broader goal of detecting *when* a person's state changes, not only *who* is at higher average risk.

## Dataset

The project uses the BRIGHTEN digital-phenotyping datasets:

| Cohort | Participants | Datapoints | Passive features | Follow-up |
|---|---:|---:|---:|---:|
| BRIGHTEN V1 | 541 | 3,007 | 37 | 12 weeks |
| BRIGHTEN V2 | 276 | 1,159 | 111 | 12 weeks |

**Analysis plan:** V1 for primary analysis, followed by V2 for reproducibility validation.

> Participant-level raw data are not redistributed in this repository.

## Analytical framework

![Research objective](assets/figure-02-research-objective.png)

1. **Participant-level sequence construction** - preserve daily ordering of mobility, communication, and device-activity features.
2. **Habitual baseline estimation** - characterize each participant's typical behavioral pattern.
3. **Within-person anomaly detection** - identify short windows in which behavior deviates from that baseline.
4. **Temporal linkage** - test whether anomaly windows precede subsequent PHQ-9 change.
5. **Robustness and replication** - vary anomaly definitions / prediction horizons and reproduce the analysis in BRIGHTEN V2.

![Sequential representation](assets/figure-03-sequential-representation.png)

## Current status

This is an ongoing study. **No final predictive-performance claim is made in this repository.** Current work focuses on anomaly definitions, time-series representation, participant heterogeneity, missingness, and temporal validation.

## Why this matters

Population-level models are useful for estimating average risk, but they can obscure clinically meaningful change within an individual. This project explores whether passive sensing can be used as a personalized monitoring signal by explicitly modeling deviations from a participant's own behavioral history.

## My contribution

- Research-question and analytical-framework design
- Participant-level time-series construction
- Passive-sensing feature analysis
- Within-person anomaly-detection design
- Temporal association analysis with subsequent PHQ-9 change
- Reproducibility design using BRIGHTEN V2
- Visualization and manuscript preparation

## Project outputs

- [`outputs/methodology-seminar-public-excerpt.pdf`](outputs/methodology-seminar-public-excerpt.pdf) - curated public excerpt from the Sep. 2026 SI Lab seminar; it documents the methodological transition toward passive-only PHQ-9 prediction and sequential representation.
- Original BRIGHTEN participant-level data are not included.

## Repository scope

This repository is a **research portfolio repository**. It documents the study design, selected figures, and public-safe research artifacts. Analysis code will only be published when it can be released without violating dataset-use restrictions and after the analysis interface is stabilized.

---

**Junha Won**  
Ajou University, Department of Industrial Engineering  
[Portfolio](https://juna0926.github.io/Portfolio/) · [GitHub](https://github.com/Juna0926)
