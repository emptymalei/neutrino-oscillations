---
title: "Background Matter Basis"
description: "Background Matter Basis"
lead: ""
date: 2020-04-20T11:53:07+02:00
lastmod: 2020-04-20T11:53:07+02:00
draft: false
menu:
  book:
    parent: "2. Neutrino Oscillations with Oscillatory Matter Profile"
images: []
weight: 320
toc: false
---

For a uniform matter density $\lambda(r) = \lambda_0$, one can define a matter basis in which the Hamiltonian is diagonalized:
{{<m>}}
\begin{equation}
\mathsf H^{(\mm)}  = \mathsf U^\dagger \mathsf H^{(\ff)} \mathsf U = -\frac{\omega_\mm}{2} \sigma_3,
\label{chap:matter-sec:background-eqn:hamiltonian-matter-basis}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
\mathsf U = \begin{pmatrix}
\cos \theta_\mm & \sin \theta_\mm \\
\sin\theta_\mm & \cos \theta_\mm
\end{pmatrix}
\end{equation}
{{</m>}}
with
{{<m>}}
\begin{equation}
\theta_{\mathrm{m}}= \frac{1}{2} \arctan\left(
\frac{\sin 2\theta_{\mathrm v}}{ \cos 2\theta_{\mathrm v} - \lambda_0/\omega_{\mathrm v} } \right),
\label{chap:matter-sec:background-eqn:thetam-expression}
\end{equation}
{{</m>}}
and
{{<m>}}
\begin{equation}
\omega_{\mathrm{m}} = \omega_{\mathrm{v}} \sqrt{ ( \lambda_0/\omega_{\mathrm{v}} - \cos (2\theta_{\mathrm{v}}) )^2 + \sin^2(2\theta_{\mathrm{v}}) }
\label{chap:matter-sec:background-eqn:omegam}
\end{equation}
{{</m>}}
is the neutrino oscillation frequency in matter.

In the rest of the chapter, I will consider the matter profiles of the form
{{<m>}}
\begin{equation}
    \lambda(r) = \lambda_0 + \delta \lambda(r),
    \label{eq-general-matter-profile}
\end{equation}
{{</m>}}
where $\delta \lambda(r)$ describes the fluctuation of the matter density. I will use the background matter basis defined in Eqn. \ref{chap:matter-sec:background-eqn:hamiltonian-matter-basis},  Eqn. \eqref{chap:matter-sec:background-eqn:thetam-expression} and Eqn. \eqref{chap:matter-sec:background-eqn:omegam}. In this basis, the Hamiltonian reads
{{<m>}}
\begin{equation}
    \mathsf H^{(\mathrm{m})} = -\frac{\omega_\mm}{2} \sigma_3 + \frac{1}{2} \delta\lambda(r) \cos 2\theta_{\mathrm m} \sigma_3
     - \frac{1}{2} \delta\lambda(r) \sin 2\theta_{\mathrm m} \sigma_1.
    \label{eq-hamiltonian-bg-matter-basis-general}
\end{equation}
{{</m>}}

In this chapter, I will focus on the transition probability between the background matter eigenstates
{{<m>}}
\begin{equation}
    \begin{pmatrix}
        \ket{\nu_{\mathrm L}} \\
        \ket{\nu_{\mathrm H}}
    \end{pmatrix} = \mathsf U^\dagger \begin{pmatrix}
        \ket{\nu_{\mathrm e}} \\
        \ket{\nu_{\mathrm x}}
    \end{pmatrix}.
\end{equation}
{{</m>}}
Given this transition probability, it is trivial to calculate the conversion between flavors.

All the numerical examples in this chapter are calculated with $\sin^2(2\theta_{\mathrm v}) = 0.093$ and $\omega_{\vv} = 1.3\times 10^{-16}\mathrm{MeV}$ [^Patrignani:2016xqp].

[^Patrignani:2016xqp]: {{< ref key="Patrignani:2016xqp">}}