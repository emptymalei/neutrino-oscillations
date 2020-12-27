---
title: "Rabi Basis"
description: "Rabi Basis"
lead: ""
date: 2020-04-20T11:53:07+02:00
lastmod: 2020-04-20T11:53:07+02:00
draft: false
menu:
  book:
    parent: "2. Neutrino Oscillations with Oscillatory Matter Profile"
images: []
weight: 350
toc: false
---

Previously I have ignored the oscillating $\sigma_3$ terms in the Hamiltonian such as in Eqn. \eqref{chap:matter-sec:single-fequency-eq:hamiltonian-bg-matter-basis-single-frequency}. Using the Jacobi-Anger expansion, J. Kneller et al. showed that these terms result in an infinite number of resonance conditions. In the rest of the chapter, I will present a much simpler derivation of their results from the perspective of Rabi oscillations. For this purpose I will define a new basis called Rabi basis
{{<m>}}
\begin{equation}
\begin{pmatrix} \ket{\nu_{\mathrm{r1}}}\\ \ket{\nu_{\mathrm{r2}}} \end{pmatrix} =  \mathsf{U}^\dagger \begin{pmatrix} \ket{\nu_{\mathrm{L}}} \\ \ket{\nu_{\mathrm{H}}} \end{pmatrix},
\label{eq-rabi-basis}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
\mathsf{U} =  \begin{pmatrix} e^{-\ri \eta (r)} & 0 \\  0 & e^{\mathrm i \eta (r)}  \end{pmatrix}.
\label{eq-rabi-transformation}
\end{equation}
{{</m>}}
The unitary transformation in Eqn.~\eqref{eq-rabi-transformation} is a rotation in flavor space about the third axis.
It commutes with $\sigma_3$ terms in the Hamiltonian, but, due to its dependence on $r$, the left side of the Schr\"{o}dinger equation obtains an extra term:
{{<m>}}
\begin{align*}
    &\begin{pmatrix}  \frac{\mathrm d\eta}{\mathrm dr}  & 0 \\ 0 & - \frac{\mathrm d\eta}{\mathrm d r}  \end{pmatrix} \begin{pmatrix} \psi_{\mathrm R1} \\ \psi_{\mathrm R2} \end{pmatrix} + \mathrm i \frac{\mathrm d}{\mathrm dr} \begin{pmatrix} \psi_{\mathrm R1} \\ \psi_{\mathrm R2} \end{pmatrix} \\
    =& \left[ -\frac{\omega_{\mathrm m} }{2} \sigma_3  + \frac{\delta \lambda}{2} \cos 2\theta_{\mathrm m}  \sigma_3  - \frac{\delta \lambda}{2} \sin 2\theta_{\mathrm m} \begin{pmatrix} 0 & e^{2\mathrm i\eta} \\ e^{-2 \mathrm i\eta } & 0 \end{pmatrix}   \right] \begin{pmatrix} \psi_{\mathrm R1} \\ \psi_{\mathrm R2} \end{pmatrix}.
\end{align*}
{{</m>}}
The oscillating $\sigma_3$ terms in Hamiltonian can be eliminated by choosing $\eta(r)$ properly, i.e.,
{{<m>}}
\begin{equation}
    \eta(r) - \eta(0) =  \frac{\cos 2\theta_{\mathrm{m}}}{2} \int_0^r \delta\lambda (\tau) \dd\tau.
\end{equation}
{{</m>}}
With this definition, the Schr\"{o}dinger equation simplifies:
{{<m>}}
\begin{equation}
    \ri \frac{\dd}{\dd r} \begin{pmatrix} \psi_{\mathrm r1} \\ \psi_{\mathrm r2} \end{pmatrix} = \left[ - \frac{\omega_{\mathrm m}}{2} \sigma_3 - \frac{\delta \lambda}{2} \sin 2\theta_{\mathrm m} \begin{pmatrix} 0 & e^{2\ri\eta} \\ e^{-2 \ri \eta } & 0 \end{pmatrix}\right] \begin{pmatrix} \psi_{\mathrm r1} \\ \psi_{\mathrm r2} \end{pmatrix}.
    \label{chap:matter-sec:jacobi-subsec:rabi-basis-eqn:eom-rabi-basis-matter}
\end{equation}
{{</m>}}
Because the states $\ket{\nu_{r1}}$ and $\ket{\nu_{r2}}$ are related to $\ket{\nu_{\mathrm L}}$ and $\ket{ \nu_{\mathrm H} }$ by phase factors only, the transition probability between the former two states is the same as that between the latter.