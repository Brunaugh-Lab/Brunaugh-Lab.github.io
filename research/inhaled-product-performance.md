---
layout: page
title: Inhaled Product Performance
subtitle: Prediction and optimization of inhaled product performance
description: Distribution-sensitive measurements and explicit inference frameworks for understanding inhaled particle performance.
permalink: /research/inhaled-product-performance/
---

[← Back to Research](/research/)

<figure class="research-figure">
  <img src="/images/research/wasserstein-graphical-abstract.png" alt="Graphical abstract showing Wasserstein distance framework for quantifying dispersibility across dry powder inhaler formulations." loading="lazy" decoding="async">
  <figcaption>The Wasserstein distance framework compares entire particle size distributions to quantify how closely an inhaler-generated aerosol approaches a powder's intrinsic dispersion limit.</figcaption>
</figure>

## The Problem

The tools we use to evaluate inhaled drug products were designed for convenience, not fidelity. Cascade impaction — the regulatory gold standard — collapses rich aerodynamic size distributions into scalar summaries like fine particle fraction and mass median aerodynamic diameter. Dissolution testing for inhaled products remains poorly standardized, with no consensus method for capturing how particles dissolve and transform in the thin fluid layers that line the airways.

These summary statistics discard distributional information that carries mechanistic significance. Two formulations can produce identical fine particle fractions while exhibiting fundamentally different dispersion pathways. A dissolution profile measured under sink conditions may bear no relationship to what happens in a mucus-lined airway where fluid volumes are vanishingly small and drug-barrier interactions dominate.

The result is that formulation scientists optimize against metrics that may not predict clinical performance, and device engineers cannot distinguish between device-limited and formulation-limited dispersion.

## Our Approach

We are building physically grounded, distribution-sensitive analytical frameworks that preserve the information conventional metrics discard.

**Wasserstein distance for aerosol dispersibility.** We introduced a framework that applies the Wasserstein distance (Earth Mover's Distance) to quantify how closely an inhaler-generated aerosol approaches a powder's intrinsic dispersion limit. Unlike scalar metrics, this approach compares entire particle size distributions, capturing formulation-, device-, and flow-dependent differences in dispersibility that visual inspection of size distributions alone cannot separate. The metric is formulation-agnostic, physically interpretable, and works with standard laser diffraction data. We released the analysis toolkit as open-source software.

**Dynamic observation of particulate transformation.** We are developing DiffractoMorph, a framework that combines time-resolved, multichannel angular-scattering measurements with dissolved-phase mass balance to observe particulate systems as they change in biorelevant media. A detector response alone does not uniquely identify whether particles dissolved, changed in number, aggregated, or reorganized. We therefore use calibrated observation operators, controlled perturbations, and minimum-sufficient models to determine which explanations the measurements support — and to state clearly when competing mechanisms remain unresolved.

**From screening to prediction.** The long-term goal is a measurement-to-prediction pipeline: use distribution-sensitive characterization and explicit measurement models to build physically grounded predictions of product performance, while preserving the boundary between direct observation and model-dependent mechanism.

## Selected Publications & Tools

- Xia G, Dechayont B, Che L, Comfort I, Brunaugh AD. A distribution-based metric for quantifying dispersibility in dry powder inhalers. *Pharmaceutics*, 2026.
- [Dispersibility Analysis Toolkit](https://github.com/Brunaugh-Lab/dispersibility-analysis) — open-source R package
- [Raw Laser Diffraction Datasets](https://doi.org/10.7302/nwc8-9f06) — Deep Blue Data repository
