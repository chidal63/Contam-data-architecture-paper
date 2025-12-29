Project status — Occurrence data architecture and uncertainty-driven exposure

Scope and objective

This repository accompanies a research manuscript investigating how structural properties of occurrence data architectures—rather than contaminant-specific behaviour or exposure modelling choices—drive uncertainty in dietary exposure assessment and, in turn, function as governance signals within food systems.

The objective is not to re-estimate exposure or to compare contaminants toxicologically, but to identify and document architecture-level constraints that systematically shape exposure metrics upstream of modelling.

⸻

Conceptual framework

The work is structured around the hypothesis that:

Uncertainty-dominated exposure estimates emerge as a structural property of how occurrence data are generated, encoded, aggregated and propagated, independently of contaminant identity.

To test this hypothesis, we analyse a limited number of deliberately selected case studies, each representing a distinct monitoring architecture and governance logic within contemporary food systems.

⸻

Case selection rationale (anti–cherry-picking)

Contaminants and datasets were selected by architectural function, not by chemical class, hazard profile, or availability of data.
The selection spans contrasting positions along the occurrence-to-exposure pipeline, allowing us to probe whether uncertainty-driven exposure is a general structural phenomenon.

We explicitly avoid catalogue-style analyses of multiple similar contaminants, as this would dilute architectural inference without increasing explanatory power.

⸻

Datasets included in the analysis

1. Aflatoxins (AFLA) — Mature benchmark

Role in the study
Aflatoxins are used as a best-case benchmark: a mature, long-established, and harmonised monitoring system with extensive regulatory experience.

Why included
	•	High analytical maturity and long monitoring history
	•	Large, curated datasets with explicit left-censoring information
	•	Strong governance relevance (trade, infant foods, carcinogenicity)

Analytical focus
	•	Prevalence of left-censoring (%LCD)
	•	Inflation of UB/LB exposure estimates
	•	Sensitivity of exposure metrics to reporting limits

Purpose
To demonstrate that architecture-driven uncertainty emerges even under best-case monitoring conditions, ruling out immaturity or poor data quality as primary explanations.

⸻

2. Nitrosamines — Emerging, unstable architecture

Role in the study
Nitrosamines represent an emerging contaminant group with recent regulatory attention and heterogeneous monitoring practices.

Why included
	•	High current policy relevance
	•	Fragmented endpoint semantics (multiple species)
	•	Heterogeneous analytical sensitivity and reporting practices

Analytical focus
	•	Left-censoring and UB/LB behaviour where available
	•	Loss of resolution imposed by aggregation (e.g. TERM_LEVEL_CONC vs nominal FoodEx level)
	•	Evidence of architecture-driven uncertainty under conditions of monitoring instability

Purpose
To probe whether the same structural constraints observed for mature contaminants also arise in emerging and still-evolving monitoring regimes.

⸻

3. Perchlorate — Exposure-facing governance case

Role in the study
Perchlorate is used as an exposure-facing case, explicitly linking occurrence data architecture to dietary exposure outputs.

Why included
	•	Non-mycotoxin, non-natural contaminant
	•	Availability of occurrence data directly connected to exposure results
	•	Clear relevance for population-level exposure assessment and standard-setting

Analytical focus
	•	Relationship between occurrence uncertainty and contribution to dietary exposure
	•	Identification of food categories that dominate exposure under uncertainty-dominated metrics

Purpose
To demonstrate that architecture-driven uncertainty propagates into exposure outputs that directly inform food-system decisions, closing the loop between data structure and governance relevance.

⸻

4. Seaweeds and halophytes (heavy metals and iodine) — End-to-end architecture

Role in the study
This case provides an end-to-end view of the data pipeline, using raw occurrence data and curated food-level data from the same scientific opinion.

Why included
	•	Availability of both raw (record-level) and curated occurrence data
	•	Same contaminants, same context, different architectural layers

Analytical focus
	•	Evidence of uncertainty already encoded at the point of data generation
	•	Amplification or transformation of uncertainty through curation and aggregation

Purpose
To isolate how uncertainty is progressively encoded and reshaped along the occurrence-to-exposure pipeline, independent of contaminant identity.

⸻

Analytical strategy (high-level)

Across all cases, analyses are restricted to a common set of architecture-relevant diagnostics, applied only where supported by the data:
	•	Left-censoring prevalence (ND / %censored)
	•	UB/LB inflation (or equivalent proxies)
	•	Reporting limit heterogeneity
	•	Resolution loss due to aggregation or semantic constraints

No contaminant-specific exposure re-modelling is performed.

⸻

Current status
	•	Dataset selection finalised
	•	Conceptual framework and case rationale fixed
	•	Script development focuses on:
	•	reproducible ingestion and cleaning
	•	transparent calculation of architecture-level metrics
	•	generation of figures supporting the manuscript

This repository documents how results are obtained, not alternative analytical choices that are outside the scope of the manuscript.

⸻

Se vuoi, prossimo passo naturale:
	•	trasformare questo STATUS in un README.md minimale con struttura delle cartelle (data/, scripts/, figures/),
	•	oppure preparare una roadmap degli script (ordine di esecuzione, input/output attesi).
