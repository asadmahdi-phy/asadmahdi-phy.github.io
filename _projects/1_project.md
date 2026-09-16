---
layout: page
title: "Testing General Relativity with Gravitational Waves"
description: "Studying how merger-ringdown modifications bias parameterized inspiral tests for LISA."
img: assets/img/gravitational_wave_project.jpg
importance: 2
category: research
related_publications: false
---

## Project overview

During my research internship at the **Laboratoire des Deux Infinis de Toulouse (L2IT)**, I worked with **Sylvain Marsat** and **Manuel Piarulli** on systematic biases in gravitational-wave tests of general relativity (GR). We studied simulated signals from massive black-hole binaries relevant to the future **Laser Interferometer Space Antenna (LISA)**.

Our question was specific: **if a signal has a modified merger-ringdown but a GR inspiral, can an analysis mistakenly recover a nonzero inspiral-deviation parameter?** To investigate this, we constructed signals with controlled ringdown modifications and analysed them with models that allowed deviations only in the inspiral sector. We then compared approximate predictions of the resulting parameter biases with full Bayesian parameter estimation.

## Constructing the modified signals

We used an aligned-spin binary with total mass $M = 10^6 M_\odot$, mass ratio $q = 4$, and component spins $\chi_1 = \chi_2 = 0.5$. The waveform included six spherical-harmonic modes: $(2,2)$, $(2,1)$, $(3,3)$, $(4,4)$, $(4,3)$, and $(5,5)$.

The ringdown modification was introduced through **pSEOBNRv5HM**, using the parameterized ringdown functionality available in **pySEOBNR**. We changed the oscillation frequency and damping time associated with the dominant $(2,2)$ mode,

$$
\omega_{22} \rightarrow \omega_{22}(1+\delta\omega_{22}),
\qquad
\tau_{22} \rightarrow \tau_{22}(1+\delta\tau_{22}),
$$

while retaining the GR inspiral dynamics and leaving the other modes' ringdown parameters unchanged. We varied the two fractional deviations together,

$$
\delta\omega_{22}=\delta\tau_{22}
\in \{0,10^{-4},10^{-3},10^{-2},0.1\}.
$$

For each case, we generated the time-domain modes, applied a Planck taper to reduce edge effects, and Fourier transformed the signals. This gave us both the amplitude and phase changes produced by the ringdown modification.

An important part of the work was separating the intended modification from differences between waveform implementations. Our recovery model, **SEOBNRv5HMROM**, is a fast frequency-domain reduced-order model. Even with no ringdown deviation, its waveform is not numerically identical to the Fourier-transformed time-domain waveform. Directly comparing the two would therefore mix the injected effect with their baseline differences.

To reduce this problem, we extracted a complex multiplier from the modified and unmodified pSEOBNR waveforms. For each mode, it combined their amplitude ratio and phase difference,

$$
\mathcal{M}_{\ell m}(f)
=\frac{A^{\mathrm{dev}}_{\ell m}(f)}{A^{\mathrm{GR}}_{\ell m}(f)}
\exp\!\left[i\Delta\Phi_{\ell m}(f)\right].
$$

After removing a constant phase offset and interpolating onto the ROM frequency grid, we applied this multiplier to each ROM mode's contribution to the LISA signal. The injection and recovery then shared a ROM baseline, with the injection carrying the relative waveform change extracted from pSEOBNR. In the zero-deviation limit, the multiplier reduces to unity.

## Recovering the signal with inspiral deviations

We constructed the LISA **time-delay interferometry (TDI)** signals using **lisabeta**, accounting for the detector response before comparing waveforms. We also aligned the waveforms in time, orbital phase, and polarization, and evaluated their agreement using noise-weighted overlaps.

The recovery waveform retained a GR merger-ringdown but included one active **Flexible Theory-Independent (FTI)** inspiral parameter in each run. The tested parameters included post-Newtonian phase coefficients and corrections associated with spin-induced quadrupole moments and gravitational-wave tails. The ordinary source parameters were allowed to vary along with the selected FTI parameter.

This setup deliberately gave the recovery model an incomplete description of the injected signal. It could adjust masses, spins, and other source parameters, or shift the active inspiral coefficient, but it could not directly reproduce the injected ringdown modification. All injected FTI coefficients were zero, so a recovered displacement measured how the model responded to the missing merger-ringdown physics.

## Estimating and checking the parameter biases

We first used the **Cutler-Vallisneri (CV) formalism** to estimate the systematic shifts. We calculated the residual between the injection and the reference recovery waveform, evaluated waveform derivatives numerically, and constructed the Fisher matrix. The leading-order bias is

$$
\Delta\lambda^i_{\mathrm{CV}}
= (\Gamma^{-1})^{ij}
\left\langle \partial_j h\mid\delta h\right\rangle,
\qquad
\delta h=h_{\mathrm{inj}}-h_{\mathrm{rec}}.
$$

Here, $\boldsymbol{\lambda}$ includes the source parameters and the active FTI coefficient. We compared each predicted shift with its Fisher uncertainty, $\sigma_i=\sqrt{(\Gamma^{-1})^{ii}}$, to assess its size relative to the statistical precision of the measurement.

We then performed **Bayesian parameter estimation**, examining likelihood traces, marginalized posteriors, and joint parameter distributions. We measured posterior-median displacements from the injected values and compared them with the CV predictions. These were comparisons of parameter recovery within each model, rather than comparisons of Bayesian evidence between models.

The GR null tests were essential checks. A direct comparison of the time-domain GR waveform with the ROM gave biases below $0.5\sigma$. With the multiplier construction, the reported CV null-test biases fell below approximately $10^{-3}\sigma$. The Bayesian null test also recovered an FTI posterior consistent with zero. These checks established the behavior of the pipeline at zero deviation, although they do not independently rule out numerical errors in every modified injection.

## What we found

**A merger-ringdown modification can shift both the recovered source parameters and an inspiral-deviation coefficient.** The size and sign of the FTI shift depended on which coefficient was allowed to vary, reflecting its frequency dependence and its correlations with the other parameters.

For the **1% ringdown modification**, several parameter shifts exceeded their statistical uncertainties. In the recovery with the spin-induced quadrupole parameter $\delta\kappa_s$ active, for example, the mass ratio moved from $4$ to about $3.93$, and the effective spin moved from $0.50$ to about $0.44$. The $\delta\kappa_s$ displacement was approximately $-1.2\sigma$. This was not a significant detection of modified inspiral physics, but it showed how an apparent inspiral shift could arise without introducing that effect into the signal.

For deviations between **$10^{-4}$ and $10^{-2}$**, the CV predictions broadly followed the direction and approximate size of the normalized Bayesian posterior shifts. The main discrepancies involved the time parameter. At $10^{-4}$, the shifts were below approximately $0.15\sigma$ for the configuration studied.

The **10% modification** required a different conclusion: the Bayesian runs did not converge to reliable posterior distributions. Their likelihood traces continued to evolve, and the posteriors were fragmented or multimodal. We therefore excluded this case from the quantitative CV–Bayesian comparison.

## Interpretation and scope

The result concerns how parameters are inferred from the complete signal. Changes in masses and spins that help accommodate a modified ringdown also change the predicted inspiral. An FTI correction can compensate for part of that change while all parameters are fitted together. A nonzero inspiral coefficient therefore does not, by itself, identify where the underlying waveform modification occurred.

This study used one binary configuration, modified only the dominant mode, and varied its frequency and damping time together. The results establish this bias mechanism for the cases tested; they do not provide a universal deviation threshold for LISA. A natural extension is to vary the ringdown modifications independently and include them in the recovery alongside the inspiral parameters, testing whether accounting for the injected physics brings the recovered FTI coefficients back towards zero.
