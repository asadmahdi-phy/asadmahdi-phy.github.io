---

layout: page
title: "Testing General Relativity with Gravitational Waves"
description: "Can merger-ringdown deviations be misinterpreted as deviations in the inspiral?"
img: assets/img/gravitational_wave_project.jpg
importance: 2
category: research
related_publications: false
---------------------------

## Project overview

During my research internship at the **Laboratoire des Deux Infinis de Toulouse (L2IT)**, I worked with **Sylvain Marsat** and **Manuel Piarulli** on tests of general relativity using gravitational waves from massive black-hole binaries. The project was motivated by the future **Laser Interferometer Space Antenna (LISA)**, which will observe massive black-hole mergers with exceptionally high signal-to-noise ratios.

A binary black-hole gravitational-wave signal contains three connected stages: inspiral, merger, and ringdown. Parameterized tests of gravity often associate particular deviation parameters with one of these stages. Inspiral tests, for example, introduce corrections to the post-Newtonian phase, while ringdown tests modify the frequencies or damping times of the remnant black hole’s quasinormal modes.

However, the full signal is analysed simultaneously. A modelling error or an unmodelled physical effect in one part of the waveform can therefore influence parameters associated with another part.

The central question of our project was:

> **Can a deviation introduced only in the merger-ringdown sector be incorrectly recovered as a deviation in the inspiral phase?**

## Injection-recovery framework

We studied this problem using an **injection-recovery framework**. The injection represents the signal produced by nature, while the recovery waveform represents the model used to analyse the signal.

For the injection, we constructed a waveform with a general-relativistic inspiral but a modified merger-ringdown. The modification changed the characteristic frequency and damping time of the ringdown modes,

$$
\omega \rightarrow \omega(1+\delta\omega),
\qquad
\tau \rightarrow \tau(1+\delta\tau).
$$

Several values of the fractional deviations (\delta\omega) and (\delta\tau) were considered to determine how the recovered parameters changed with the strength of the modification.

The recovery model was constructed with the opposite assumption. Its merger-ringdown sector followed general relativity, while one **Flexible Theory-Independent (FTI)** inspiral-phase parameter was allowed to vary in each analysis. FTI parameters modify individual post-Newtonian contributions to the inspiral phase without selecting a particular alternative theory of gravity.

The structure of the analysis was therefore

$$
\text{Injection: GR inspiral + modified merger-ringdown},
$$

$$
\text{Recovery: modified inspiral + GR merger-ringdown}.
$$

This deliberate inconsistency allowed us to test whether the recovery model would compensate for missing merger-ringdown physics by shifting an inspiral-deviation parameter away from its general-relativistic value.

## Measuring systematic bias

We investigated the resulting parameter shifts using full Bayesian parameter estimation and the **Cutler-Vallisneri systematic-bias formalism**.

If the true signal and the approximate recovery model differ by

$$
\delta h = h_{\mathrm{true}}-h_{\mathrm{approx}},
$$

the leading-order shift in the inferred parameters is

$$
\Delta\theta^{i}
================

\left(\Gamma^{-1}\right)^{ij}
\left\langle
\partial_j h
\middle|
\delta h
\right\rangle,
$$

where (\Gamma_{ij}) is the Fisher information matrix. We compared this systematic shift with the statistical uncertainty,

$$
\sigma_i
========

\sqrt{\left(\Gamma^{-1}\right)_{ii}}.
$$

The ratio

$$
\frac{|\Delta\theta^i|}{\sigma_i}
$$

measures the importance of the modelling bias. A value close to or greater than one means that the systematic displacement is comparable to, or larger than, the expected statistical uncertainty.

Geometrically, the recovery model defines a manifold of possible waveforms. A signal containing an unmodelled merger-ringdown deviation does not lie exactly on this manifold. Parameter estimation therefore selects the closest available waveform, and the displacement of its parameters from the true values appears as a systematic bias.

## Main findings

Our analysis showed that a deviation confined to the merger-ringdown can bias the recovery of inspiral-sector parameters. The recovery model can partially absorb the missing late-time physics by shifting an FTI inspiral parameter away from its general-relativistic value.

The effect was not identical for all FTI parameters. Each parameter modifies a different frequency-dependent contribution to the inspiral phase, so different parameters have different abilities to compensate for the waveform discrepancy produced by the modified merger-ringdown.

For some injected deviations and FTI parameters, the systematic shift became comparable to the corresponding statistical uncertainty. The analysis could therefore indicate an apparently significant inspiral deviation even though the physical modification had been introduced only in the merger-ringdown.

We also performed a null test with no injected merger-ringdown deviation. In this case, the recovered FTI parameters remained close to their general-relativistic values. This confirmed that the biases observed in the modified cases were associated with the intended waveform inconsistency rather than with the numerical procedure itself.

For sufficiently small deviations, the Cutler-Vallisneri prediction reproduced the direction and approximate magnitude of the shifts found through parameter estimation. At larger deviations, nonlinear effects and broader correlations between parameters became increasingly important.

## Why this matters for LISA

LISA is expected to observe massive black-hole mergers with very high signal-to-noise ratios. Such observations will provide extremely small statistical uncertainties and create an unprecedented opportunity to test gravity in the strong-field regime.

At the same time, high measurement precision makes waveform systematics more important. Statistical errors decrease as the signal becomes stronger, but modelling errors do not necessarily decrease. Even a relatively small mismatch between the true signal and the recovery model can therefore produce an apparently significant deviation from general relativity.

Our results show that an inspiral-deviation parameter cannot always be interpreted as a measurement of inspiral physics alone. A nonzero value could instead be caused by missing or inaccurate merger-ringdown physics. Tests applied to the inspiral, merger, and ringdown are connected through the global waveform fit and through correlations in parameter space.

Reliable tests of gravity with LISA will therefore require accurate waveform models across the complete inspiral-merger-ringdown signal, frameworks that allow deviations in more than one waveform sector, consistency checks between inspiral and merger-ringdown tests, and careful comparisons between systematic and statistical uncertainties.

This project addresses a central challenge in precision gravitational-wave astronomy: distinguishing a genuine failure of general relativity from an apparent deviation produced by an incomplete waveform model. Controlling these cross-sector biases will be essential for converting LISA’s exceptional measurement precision into reliable conclusions about the fundamental nature of gravity.
