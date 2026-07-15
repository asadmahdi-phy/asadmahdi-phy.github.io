---
layout: page
title: Anisotropic Quenched Noise in the $\phi^4$ Model
description: Studying how spatially anisotropic frozen disorder affects critical behaviour and universality in the $\phi^4$ model.
img: assets/img/nordita_project.jpg
importance: 1
category: research
related_publications: false
---

At Nordita, I am working with Dr. Dhrubaditya Mitra on a question at the intersection of statistical field theory and phase transitions: what happens to critical behaviour when spatially anisotropic, frozen disorder is introduced into the $\phi^4$ model? Specifically, does this form of frozen roughness change the universal properties of the paramagnetic-to-ferromagnetic phase transition?

## Why universality matters

Near a critical point, the correlation length becomes very large compared with the microscopic length scales of the system. Consequently, many microscopic details cease to influence the large-scale behaviour. This is the origin of universality: systems that appear completely different microscopically can display identical behaviour near a critical point.

Such systems belong to the same universality class and share the same critical exponents and scaling functions.

The \(\phi^4\) model is one of the simplest field-theoretic descriptions of this type of phase transition. For an \(n\)-component order-parameter field \(\boldsymbol{\phi}(\mathbf{x})\), the clean Hamiltonian is

\begin{equation}
\mathcal{H}_0[\boldsymbol{\phi}]
=
\int d^d x
\left[
\frac{1}{2}
\left(\nabla\boldsymbol{\phi}\right)^2
+
\frac{\tau}{2}\boldsymbol{\phi}^2
+
\frac{u}{4!}
\left(\boldsymbol{\phi}^2\right)^2
\right].
\end{equation}

The parameter \(\tau\) controls the distance from the critical point. At the mean-field level, a phase transition occurs when \(\tau\) changes sign.

For \(\tau>0\), the equilibrium state is

\begin{equation}
\boldsymbol{\phi}=0,
\end{equation}

which corresponds to the paramagnetic phase. For \(\tau<0\), the system develops a nonzero order parameter, corresponding to the ferromagnetic phase.

Mean-field theory, however, neglects fluctuations. These fluctuations become increasingly important near criticality. The renormalization group is therefore required to determine the actual large-scale critical behaviour.

## Adding frozen disorder

The central modification considered in this project is the introduction of anisotropic quenched disorder. Quenched disorder is a form of frozen randomness that does not evolve on the timescale of the order-parameter fluctuations.

It may represent impurities, structural defects, or spatially irregular interactions embedded in the material. Unlike thermal noise, which fluctuates dynamically, quenched disorder remains fixed while the physical system equilibrates.

Thermodynamic quantities must first be calculated for each fixed disorder realization. Only afterward is an average over the different disorder configurations performed.

The disorder can be introduced through an anisotropic coupling to the gradient sector,

\begin{equation}
\mathcal{H}_{\mathrm{dis}}
=
\frac{1}{2}
\int d^d x\,
\delta K_{ij}(\mathbf{x})
\,
\partial_i\boldsymbol{\phi}
\cdot
\partial_j\boldsymbol{\phi}.
\end{equation}

Here, \(\delta K_{ij}(\mathbf{x})\) is a random tensor describing local variations in the stiffness of the field. Its mean is taken to vanish,

\begin{equation}
\overline{\delta K_{ij}(\mathbf{x})}=0,
\end{equation}

while its two-point correlation function is written as

\begin{equation}
\overline{
\delta K_{ij}(\mathbf{x})
\delta K_{kl}(\mathbf{x}')
}
=
\Delta_{ij,kl}
C(\mathbf{x}-\mathbf{x}').
\end{equation}

The tensor \(\Delta_{ij,kl}\) describes the directional structure of the disorder, while \(C(\mathbf{x}-\mathbf{x}')\) determines its spatial correlation range.

The essential feature is that the frozen disorder treats different spatial directions differently.

## Mean-field analysis

The first stage of the project is a mean-field analysis. This allows us to investigate whether the disorder changes the location or basic structure of the phase transition.

For example, the disorder may modify the effective stiffness or shift the critical temperature \(T_c\). However, a shift in \(T_c\) does not by itself indicate a new universality class. The critical temperature is a non-universal quantity and generally depends on microscopic properties.

The more fundamental question is whether the disorder changes the critical exponents and the long-distance scaling behaviour.

## Disorder averaging and the replica trick

For a fixed disorder realization, the partition function is

\begin{equation}
Z[\delta K]
=
\int
\mathcal{D}\boldsymbol{\phi}\,
\exp
\left[
-\mathcal{H}
[\boldsymbol{\phi},\delta K]
\right].
\end{equation}

The disorder-averaged free energy depends on \(\overline{\ln Z}\), which is difficult to calculate directly. The standard method for handling this quantity is the replica trick,

\begin{equation}
\overline{\ln Z}
=
\lim_{N\rightarrow 0}
\frac{
\overline{Z^N}-1
}{N}.
\end{equation}

In this procedure, \(N\) copies, or replicas, of the original field are introduced. The replicated partition function is then averaged over the disorder.

After this average, the disorder generates effective interactions between different replicas. The resulting replicated Hamiltonian contains the original quartic interaction together with additional couplings determined by the strength, spatial correlation, and tensor structure of the quenched disorder.

## Renormalization-group analysis

The renormalization group is then applied to the disorder-averaged effective theory. The main question is whether the disorder couplings decrease or grow as short-distance degrees of freedom are integrated out.

Near the upper critical dimension \(d=4\), the calculation can be organized using the expansion parameter

\begin{equation}
\epsilon=4-d.
\end{equation}

Each coupling \(g_i\) has an associated beta function,

\begin{equation}
\beta_{g_i}
=
\mu
\frac{d g_i}{d\mu},
\end{equation}

where \(\mu\) is the renormalization scale.

The fixed points of the theory satisfy

\begin{equation}
\beta_{g_i}
\left(
g_1^{*},
g_2^{*},
\ldots
\right)
=
0.
\end{equation}

If the disorder coupling flows to zero, the disorder is irrelevant in the renormalization-group sense. The system then retains the universal critical behaviour of the clean \(\phi^4\) model.

If the disorder coupling instead approaches a stable nonzero fixed point, the system may belong to a new disorder-controlled universality class with modified critical exponents.

## Critical quantities

The principal critical quantities include the correlation-length exponent \(\nu\), the anomalous dimension \(\eta\), the susceptibility exponent \(\gamma\), and the order-parameter exponent \(\beta\).

Near the critical point, the correlation length behaves as

\begin{equation}
\xi
\sim
|T-T_c|^{-\nu}.
\end{equation}

At criticality, the two-point correlation function scales as

\begin{equation}
G(\mathbf{x})
\sim
\frac{1}{
|\mathbf{x}|^{d-2+\eta}
}.
\end{equation}

Since the disorder is anisotropic, it is also necessary to determine whether a single correlation length is sufficient. The correlation lengths parallel and perpendicular to a preferred direction may scale differently,

\begin{equation}
\xi_{\parallel}
\sim
|T-T_c|^{-\nu_{\parallel}},
\qquad
\xi_{\perp}
\sim
|T-T_c|^{-\nu_{\perp}}.
\end{equation}

A genuinely anisotropic fixed point would therefore produce direction-dependent critical scaling.

Alternatively, the microscopic anisotropy may become irrelevant under renormalization-group flow. In that case, rotational symmetry would effectively be restored at large length scales.

## The central question

The central question of this project is:

> How robust is universal critical behaviour against frozen, direction-dependent disturbances?

The answer depends on several properties of the system, including the strength of the disorder, the operator to which it couples, its spatial correlations, the number of components of the order parameter, and the spatial dimension.

The project follows the full theoretical development from the microscopic field theory to its macroscopic predictions. We begin with the equilibrium \(\phi^4\) Hamiltonian, introduce anisotropic quenched disorder, perform disorder averaging, derive the renormalization-group equations, and investigate the resulting fixed points and critical exponents.

The ultimate goal is to determine whether anisotropic quenched disorder merely shifts non-universal quantities such as \(T_c\), or whether it fundamentally changes the universality class of the paramagnetic-to-ferromagnetic transition.

This captures the central philosophy of the renormalization group: large-scale physics is not controlled by every microscopic detail, but by the limited number of interactions that remain relevant under coarse-graining. Whether anisotropic quenched disorder is one of these relevant interactions is the main question we are investigating.
