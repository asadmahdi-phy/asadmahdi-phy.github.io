---
layout: page
title: "Standard Sirens for Gravitational-Wave Cosmology"
description: "A Science Watch literature review of bright, dark, and spectral standard sirens, redshift inference, and selection effects in gravitational-wave cosmology."
img: assets/img/standard_sirens_overview.png
importance: 5
category: academic
permalink: /projects/standard-sirens-gw-cosmology/
date: 2026-11-21
---

# Standard Sirens for Gravitational-Wave Cosmology

**Science Watch | Bibliographic project | M2 Fundamental Physics, Aix-Marseille Université | 2026**  
**Focus:** Bright, dark, and spectral sirens; cosmological redshift inference; hierarchical Bayesian methods

## Overview

**How can gravitational-wave observations measure the expansion history of the Universe when the source redshift is not directly encoded in the waveform?** This is the central question of my Science Watch bibliographic study on *standard-siren cosmology*.

The inspiral of a compact binary provides an estimate of its **luminosity distance**, $d_L$, from the gravitational-wave (GW) amplitude. A cosmological measurement also requires its **redshift**, $z$. Unlike electromagnetic standard candles, GW standard sirens provide a distance scale without calibration through the traditional cosmic distance ladder. The challenge is to obtain redshift information in a way that is consistent with the GW data and the astrophysical population.

My reading is organized around **Pierra and Mastrogiovanni (2025), [*Gravitational Wave Cosmology: An Introduction*](https://arxiv.org/abs/2507.10597)**, and the primary literature cited therein. This page summarizes the physical ideas and statistical approaches covered in the review. It is a **bibliographic and conceptual study**, not a report of a new standard-siren parameter-estimation run.

![Conceptual routes to cosmological redshift information for standard sirens]({{ '/assets/img/standard-sirens/standard_sirens_overview.png' | relative_url }})
*Conceptual summary of the three redshift-information channels reviewed here. Bright, galaxy-catalogue dark, and spectral sirens differ in how they supply redshift information, not in how the GW signal measures luminosity distance.*

## The distance–redshift connection

At leading order, the frequency-domain inspiral amplitude depends inversely on luminosity distance, while the waveform phasing measures the **detector-frame chirp mass**:

$$
\tilde h(f)\propto \frac{\mathcal{M}_{c,\mathrm{det}}^{5/6}}{d_L}\,f^{-7/6},
\qquad
\mathcal{M}_{c,\mathrm{det}}=(1+z)\,\mathcal{M}_{c,\mathrm{src}}.
$$

The measured mass and distance are therefore insufficient, on their own, to determine a unique source redshift. In addition, the amplitude depends on binary inclination, producing a **distance–inclination degeneracy** that broadens distance uncertainties.

For a spatially flat, constant-$w$ cosmology (neglecting radiation),

$$
d_L(z;H_0,\Omega_m,w)=(1+z)\frac{c}{H_0}
\int_0^z\frac{dz'}{\sqrt{\Omega_m(1+z')^3+(1-\Omega_m)(1+z')^{3(1+w)}}}.
$$

At low redshift, this reduces approximately to $d_L\simeq cz/H_0$. Standard-siren cosmology combines a GW distance likelihood with redshift information to constrain $H_0$ and, for sufficiently informative sources and populations, other expansion parameters.

## Three approaches to standard-siren cosmology

| Approach | How redshift information enters | Main practical difficulty |
| :--- | :--- | :--- |
| **Bright sirens** | An identified electromagnetic (EM) counterpart and its host galaxy | Counterpart identification and selection effects; distance–inclination degeneracy |
| **Dark sirens (galaxy catalogue)** | A weighted statistical distribution of potential host galaxies within the GW localization | Incomplete catalogues, uncertain localization, host weighting |
| **Spectral sirens** | Features of the *source-frame* compact-binary mass distribution mapped to detector-frame masses | Population-model assumptions and potential mass-distribution evolution |

### Bright sirens: identifying the host

A bright siren has an associated electromagnetic counterpart that can identify a host galaxy, yielding a redshift measurement. **GW170817**, the binary-neutron-star merger associated with **NGC 4993**, is the standard example. Its GW distance and host-galaxy redshift made possible a direct standard-siren measurement of $H_0$ [Abbott et al. (2017)](https://doi.org/10.1038/nature24471).

The review emphasizes that this apparently straightforward combination still requires a consistent treatment of GW and EM likelihoods, source inclination, counterpart detectability, and selection biases. Electromagnetic observations can also help constrain the viewing geometry and thereby improve the inferred GW distance.

### Dark sirens: statistical host galaxies

Many GW events do not have an identified EM counterpart. For these **dark sirens**, galaxy surveys provide a distribution of candidate hosts and their redshifts inside the GW sky–distance localization volume. The cosmological analysis combines the GW likelihood with this statistical distribution, rather than assigning a single host galaxy.

Galaxy clustering provides useful redshift structure, but the inference depends on catalogue completeness, survey selection, redshift uncertainties, and assumptions about which galaxies are more likely to host mergers. A realistic analysis therefore accounts for **both catalogued galaxies and the population missing from a flux-limited survey**. The galaxy-catalogue formalism is developed in detail by [Gair et al. (2023)](https://eprints.gla.ac.uk/334400/).

### Spectral sirens: using the compact-binary mass spectrum

**Spectral sirens** extract statistical redshift information without identifying individual host galaxies. Cosmological redshift changes the relationship between intrinsic and observed masses:

$$m_{\mathrm{det}}=(1+z)m_{\mathrm{src}}.$$

If the source population has informative mass-spectrum features, such as a peak or break, a population model can help connect detector-frame masses and luminosity distances to cosmological redshifts. The note discusses broken-power-law, power-law-plus-peak, and multi-peak mass models.

The price is model dependence: changing the assumed mass spectrum or its evolution with redshift can shift inferred cosmological parameters. Importantly, the source review explains that **spectral sirens and galaxy-catalogue dark sirens are naturally described in a common merger-rate and population-inference framework**; their information can be combined rather than regarded as mutually exclusive methods.

## Hierarchical Bayesian inference and selection effects

An individual GW event has uncertain binary parameters, while cosmology and population properties are shared across events. This motivates **hierarchical Bayesian inference**, which combines event likelihoods with an astrophysical population model.

For a normalized population distribution, an illustrative likelihood *conditioned on the number of detected events* is

$$
\mathcal{L}(\{d_i\}\mid\Lambda)\propto
\prod_{i=1}^{N_{\mathrm{obs}}}
\frac{\displaystyle\int d\theta\,p(d_i\mid\theta)\,p_{\mathrm{pop}}(\theta\mid\Lambda)}
{\displaystyle\alpha(\Lambda)},
\qquad
\alpha(\Lambda)=\int d\theta\,p_{\mathrm{det}}(\theta)\,p_{\mathrm{pop}}(\theta\mid\Lambda).
$$

Here $\Lambda$ represents population and cosmological hyperparameters, $\theta$ the source parameters, and $\alpha(\Lambda)$ the **detection-efficiency correction**. The review also develops a rate-based formulation with a Poisson factor for the expected number of detections. In practical applications, event posterior samples and simulated detected injections are used to evaluate the required integrals and selection effects.

A central lesson is that **detected mergers are not an unbiased sample of all mergers**. Detector sensitivity, sky localization, galaxy-survey depth, and EM follow-up affect which events enter an analysis. Ignoring these selection effects can bias cosmological conclusions.

## Questions explored in this literature study

- What makes a compact-binary coalescence a self-calibrating distance indicator, and why does the GW signal generally not provide the redshift independently?
- Under which observational conditions is a bright-siren measurement preferable to a statistical dark-siren analysis?
- How do galaxy-catalogue incompleteness and assumptions about host-galaxy weights enter the dark-siren likelihood?
- Which source-frame mass features enable spectral-siren cosmology, and how can astrophysical population modelling become a systematic uncertainty?
- Why are hierarchical inference and detector-selection corrections essential when combining many GW events?

The unifying perspective is that **standard-siren cosmology is an inference problem connecting waveform physics, redshift information, population astrophysics, and the cosmological distance–redshift relation**. This bibliographic work complements my [strong-lensing cosmography project]({{ '/projects/abell-s1063-cosmography/' | relative_url }}): both investigate cosmological geometry, but through different observational distance measures.

## Selected bibliography

1. **Pierra, G. & Mastrogiovanni, S. (2025).** *Gravitational Wave Cosmology: An Introduction*. arXiv:2507.10597. **Main reading note**. [arXiv](https://arxiv.org/abs/2507.10597).
2. **Schutz, B. F. (1986).** *Determining the Hubble constant from gravitational wave observations*. *Nature*, **323**, 310–311. Foundational standard-siren proposal.
3. **Abbott, B. P. et al. (2017).** *A gravitational-wave standard siren measurement of the Hubble constant*. *Nature*, **551**, 85–88. Bright-siren application using GW170817. [DOI](https://doi.org/10.1038/nature24471).
4. **Gair, J. R. et al. (2023).** *The Hitchhiker's Guide to the Galaxy Catalog Approach for Dark Siren Gravitational-wave Cosmology*. *The Astronomical Journal*, **166**, 22. [Open version](https://eprints.gla.ac.uk/334400/).
5. **Mandel, I., Farr, W. M. & Gair, J. R. (2019).** *Extracting distribution parameters from multiple uncertain observations with selection biases*. *Monthly Notices of the Royal Astronomical Society*, **486**, 1086–1093. Hierarchical population inference.
6. **Mastrogiovanni, S. et al. (2024).** *ICAROGW: A python package for inference of astrophysical population properties of noisy, heterogeneous, and incomplete observations*. *Astronomy & Astrophysics*, **682**, A167. [DOI](https://doi.org/10.1051/0004-6361/202347007).
7. **Palmese, A. & Mastrogiovanni, S. (2025).** *Gravitational Wave Cosmology*. A broader review of the field. [arXiv:2502.00239](https://arxiv.org/abs/2502.00239).

*Science Watch bibliographic project, M2 Fundamental Physics, Aix-Marseille Université (2026). This page summarizes literature and methodology; it does not present newly derived observational constraints.*
