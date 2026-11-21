---
layout: page
title: "Strong-Lensing Cosmography with Abell S1063"
description: "Gravitational-lensing constraints on cosmology from multiple-image systems in the galaxy cluster Abell S1063."
img: assets/img/cluster_mass_map.jpg
importance: 4
category: academic
permalink: /projects/abell-s1063-cosmography/
date: 2026-11-19
---

# Strong-Lensing Cosmography with Abell S1063

**Academic project | Galaxies and Cosmology | M2 Fundamental Physics, Aix-Marseille Université | November 2026**  
**Supervisor:** Dr. Eric Jullo, Laboratoire d'Astrophysique de Marseille (LAM)  
**Tools:** Python, Jupyter, Lenstool, BayeSys, emcee, NumPy, SciPy, Astropy, Matplotlib, and `corner`

## Overview

Can a single galaxy cluster constrain the matter density of the Universe and the equation of state of dark energy? I explored this question using **strong gravitational lensing by Abell S1063** (also known as RXC J2248.7−4431), a massive galaxy cluster at redshift **$z_L \simeq 0.348$**.

When a background galaxy is multiply imaged by a foreground cluster, the image positions depend on both the cluster's gravitational potential and the angular-diameter distances between the observer, lens, and source. Multiple source galaxies at different redshifts therefore offer a way to probe cosmology, provided that the cluster mass distribution is sufficiently well modelled.

The project focused on two parameters in a spatially flat, constant-$w$ cosmology:

- **$\Omega_m$:** the present-day matter density parameter.
- **$w_X$:** the dark-energy equation-of-state parameter, with $w_X=-1$ corresponding to a cosmological constant.

My aim was not just to produce posterior contours, but to test **how much information the image geometry carries, how source-redshift coverage affects it, and how lens modelling and sampling choices influence the inferred constraints**.

## Physical idea

The lens equation can be written as

$$
\boldsymbol{\beta}=\boldsymbol{\theta}-
\frac{D_{LS}}{D_S}\,\hat{\boldsymbol{\alpha}}(\boldsymbol{\theta}),
$$

where $\boldsymbol{\theta}$ and $\boldsymbol{\beta}$ are the image and source angular positions, $\hat{\boldsymbol{\alpha}}$ is the deflection produced by the lens, and $D_{LS}/D_S$ is the *lensing efficiency*. This geometric factor depends on the cosmological model and the source redshift $z_S$.

For a flat universe with constant $w_X$,

$$
E(z)^2=\Omega_m(1+z)^3+(1-\Omega_m)(1+z)^{3(1+w_X)},
\qquad
\chi(z)=\frac{c}{H_0}\int_0^z\frac{dz'}{E(z')},
$$

and

$$
\frac{D_{LS}}{D_S}=1-\frac{\chi(z_L)}{\chi(z_S)}.
$$

To isolate the relative geometric information supplied by sources at different redshifts, I also studied the normalized efficiency

$$
\Xi(z_S;z_{S,\mathrm{ref}})=
\frac{[D_{LS}/D_S](z_S)}{[D_{LS}/D_S](z_{S,\mathrm{ref}})}.
$$

![Lensing efficiency as a function of source redshift]({{ '/assets/img/abell-s1063/lensing_efficiency.png' | relative_url }})
*Lensing efficiency for Abell S1063. The marked redshifts indicate the source distribution examined in the notebook.*

![Relative lensing efficiency under cosmological variations]({{ '/assets/img/abell-s1063/relative_efficiency.png' | relative_url }})
*Relative lensing efficiency, normalized at a reference source redshift. In the cosmological variations tested, the response over the observed source range was typically below about 1%, making the inference sensitive to modelling systematics.*

## What I did

### 1. Reconstructed and checked the multiple-image catalogue

I assembled and examined published multiple-image positions and source redshifts for Abell S1063, drawing on the catalogues of **Karman et al. (2017)**, **Caminha et al. (2016)**, and **Beauchesne et al. (2024)**. The catalogue was represented in Lenstool's `.mul` format, with observed sky coordinates (RA and Dec) and family identifiers. I checked the family assignments and removed duplicated entries in intermediate catalogue versions.

### 2. Built a parametric lensing workflow

Using **Lenstool**, I examined a simplified cluster-scale mass model, multiple-image predictions, the projected mass distribution, and critical curves. I compared two inference setups:

- **Fixed cosmology:** $(\Omega_m,w_X)=(0.30,-1)$, while optimizing the allowed mass-model parameters.
- **Free cosmology:** varying $\Omega_m$ and $w_X$ alongside the allowed lens-model parameters.

I used the image-plane residuals, $\chi^2$, and RMS offsets to assess how well the models reproduced the observed images. Posterior exploration was carried out with **BayeSys** and **emcee**, with corner plots used to inspect parameter distributions and degeneracies.

![Projected mass map and critical curves from Lenstool]({{ '/assets/img/abell-s1063/cluster_mass_map.png' | relative_url }})
*Projected mass map and critical-curve visualization from the Lenstool notebook.*

### 3. Tested the influence of high-redshift sources

I explored the geometric leverage supplied by extending the source-redshift range. In addition to published high-redshift families, I implemented a separate **forward-generation exercise** using a fixed fiducial lens model. A Python wrapper prepared seed catalogues, called Lenstool's image-prediction mode, converted local offsets back into sky coordinates, and filtered duplicate or inconsistent predictions before producing an augmented `.mul` catalogue.

Crucially, **forward-generated counter-images are model-dependent synthetic data**. They are useful for testing the analysis pipeline and investigating parameter recovery, but they do not provide new independent observational constraints.

## Results and interpretation

The results below are **exploratory outputs from the course project**, not validated precision measurements of cosmological parameters. The intervals are the reported 68% BayeSys posterior summaries; their interpretation is limited by posterior irregularity and convergence issues.

| Analysis | Catalogue | $\Omega_m$ | $w_X$ |
| :--- | :--- | :--- | :--- |
| Observed-image analysis | 34 images, 14 families; $1.397\le z_S\le6.107$ | $\approx 0.35^{+0.11}_{-0.12}$ | $\approx -1.28^{+0.46}_{-0.48}$ |
| Hybrid forward-generation test | 104 images, 32 families; $1.23\le z_S\le22$ | $0.351^{+0.060}_{-0.081}$ | $-1.471^{+0.445}_{-0.590}$ |

### Observed multiple-image analysis

![BayeSys cosmological posterior from the observed catalogue]({{ '/assets/img/abell-s1063/observed_corner.png' | relative_url }})
*Exploratory BayeSys posterior for the observed-image sample. The reference values $(\Omega_m,w_X)=(0.30,-1)$ are indicated in blue.*

For the observed sample, the best-fit image-plane $\chi^2$ changed from **44.21** with fixed cosmology to **42.13** when cosmology was allowed to vary. The modest improvement, together with the broad and irregular posterior and poor convergence in the emcee comparison, did not support a robust cosmological determination from this simplified model.

### Hybrid injection–recovery exercise

![BayeSys cosmological posterior from the hybrid catalogue]({{ '/assets/img/abell-s1063/hybrid_corner.png' | relative_url }})
*BayeSys posterior from a hybrid catalogue containing observed and model-generated images. Blue lines mark the fiducial input cosmology.*

The hybrid test used $(\Omega_m,w_X)=(0.30,-1)$ as the fiducial cosmology. Although the fitted $\Omega_m$ was broadly compatible with the input, the $w_X$ posterior was displaced toward more negative values. **Reliable recovery of the injected cosmology was therefore not established.** The synthetic source extension, reaching $z_S=22$, should not be interpreted as an observational detection at that redshift.

## Main lessons

This exercise clarified why strong-lensing cosmography is challenging, even for a well-studied cluster with multiply imaged sources spanning a substantial redshift range. The cosmological signal in *relative* distance ratios is small; changes in the assumed lens mass distribution can mimic changes in geometry; and posterior contours can appear informative even when the model, input catalogue, or sampler has not been fully validated.

**My main takeaway was methodological:** credible cosmological constraints require a consistent observational catalogue, a sufficiently flexible and well-tested lens model, meaningful image-position uncertainties, independent injection–recovery checks, and converged posterior sampling. A narrower posterior is not necessarily a more accurate one.

## References

1. **Caminha et al. (2022)**, *Galaxy cluster strong lensing cosmography: cosmological constraints from a sample of regular galaxy clusters*, Astronomy & Astrophysics **657**, A83. [Paper](https://doi.org/10.1051/0004-6361/202141994).
2. **Caminha et al. (2016)**, *CLASH-VLT: A highly precise strong lensing model of the galaxy cluster RXC J2248.7−4431 (Abell S1063) and prospects for cosmography*, Astronomy & Astrophysics **587**, A80. [Paper](https://doi.org/10.1051/0004-6361/201527670).
3. **Karman et al. (2017)**, *MUSE integral-field spectroscopy towards the Frontier Fields cluster Abell S1063. II. Properties of low luminosity Lyman-alpha emitters at z > 3*, Astronomy & Astrophysics **599**, A28. [Paper](https://arxiv.org/abs/1606.01471).
4. **Beauchesne et al. (2024)**, *A new step forward in realistic cluster lens mass modelling: analysis of Hubble Frontier Field Cluster Abell S1063 from joint lensing, X-ray, and galaxy kinematics data*, Monthly Notices of the Royal Astronomical Society **527**, 3246–3275. [Paper](https://doi.org/10.1093/mnras/stad3308).

*Course project completed in November 2026 under the supervision of Dr. Eric Jullo at the Laboratoire d'Astrophysique de Marseille (LAM), Aix-Marseille Université.*
