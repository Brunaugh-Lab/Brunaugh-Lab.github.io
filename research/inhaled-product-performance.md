---
layout: page
title: Inhaled Product Performance
subtitle: Prediction and optimization of inhaled product performance
permalink: /research/inhaled-product-performance/
---

[← Back to Research](/research/)

## The Problem

The tools we use to evaluate inhaled drug products were designed for convenience, not fidelity. Cascade impaction — the regulatory gold standard — collapses rich aerodynamic size distributions into scalar summaries like fine particle fraction and mass median aerodynamic diameter. Dissolution testing for inhaled products remains poorly standardized, with no consensus method for capturing how particles dissolve and transform in the thin fluid layers that line the airways.

These summary statistics discard distributional information that carries mechanistic significance. Two formulations can produce identical fine particle fractions while exhibiting fundamentally different dispersion pathways. A dissolution profile measured under sink conditions may bear no relationship to what happens in a mucus-lined airway where fluid volumes are vanishingly small and drug-barrier interactions dominate.

The result is that formulation scientists optimize against metrics that may not predict clinical performance, and device engineers cannot distinguish between device-limited and formulation-limited dispersion.

## Our Approach

We are building physically grounded, distribution-sensitive analytical frameworks that preserve the information conventional metrics discard.

**Wasserstein distance for aerosol dispersibility.** We introduced a framework that applies the Wasserstein distance (Earth Mover's Distance) to quantify how closely an inhaler-generated aerosol approaches a powder's intrinsic dispersion limit. Unlike scalar metrics, this approach compares entire particle size distributions, capturing formulation-, device-, and flow-dependent differences in dispersibility that visual inspection of size distributions alone cannot separate. The metric is formulation-agnostic, physically interpretable, and works with standard laser diffraction data. We released the analysis toolkit as open-source software.

**Laser diffraction as a proxy for particle dissolution and formation kinetics.** We are developing methods that repurpose laser diffraction — a fast, high-throughput technique already present in most formulation labs — as a real-time probe of particle dissolution and solid-state transformation. By tracking distributional changes over time rather than extracting single-point dissolution values, we can capture the kinetics of how particles dissolve, swell, aggregate, or transform in contact with biorelevant media. This approach — which we call DiffractoMorph — bridges the gap between static characterization and dynamic performance.

**From screening to prediction.** The long-term goal is a measurement-to-prediction pipeline: use distribution-sensitive characterization tools to generate the inputs that physically grounded transport models need to predict in vivo performance — replacing empirical correlations with mechanistic understanding.

## Who Works on This

This project involves Grace Xia (Wasserstein dispersibility framework, inhaler performance modeling), Nuz Dechayont (dispersibility analysis), and Linze Che (particle dissolution methods, DiffractoMorph development).

## Selected Publications & Tools

- Xia G, Dechayont B, Che L, Comfort I, Brunaugh AD. A distribution-based metric for quantifying dispersibility in dry powder inhalers. *Pharmaceutics*, 2026.
- [Dispersibility Analysis Toolkit](https://github.com/Brunaugh-Lab/dispersibility-analysis) — open-source R package
- [Raw Laser Diffraction Datasets](https://doi.org/10.7302/nwc8-9f06) — Deep Blue Data repository
