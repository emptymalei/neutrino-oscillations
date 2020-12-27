---
title: "Single-Frequency Matter Profiles Revisited"
description: "Single-Frequency Matter Profiles Revisited"
lead: ""
date: 2020-04-20T11:53:07+02:00
lastmod: 2020-04-20T11:53:07+02:00
draft: false
menu:
  book:
    parent: "2. Neutrino Oscillations with Oscillatory Matter Profile"
images: []
weight: 360
toc: false
---


Let us consider the single-frequency matter profile that we have studied in Sec. Single-Frequency Matter Profiles again. In the Rabi basis, the Hamiltonian becomes
{{<m>}}
\begin{equation}
    \mathsf H^{(\RR)} = \frac{\omega_\mm}{2} \sigma_3 - \frac{\sin 2\theta_\mm \lambda_1\cos (k_1 r)}{2} \begin{pmatrix}
        0 & e^{2\ri \eta(r)} \\
        e^{-2\ri \eta(r)} & 0
    \end{pmatrix},
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{equation}
    \eta(r) =  \frac{\lambda_1 \cos 2\theta_{\mathrm m}}{2 k} \sin (k_1 r) .
\end{equation}
{{</m>}}
With the Jacobi-Anger expansion
{{<m>}}
\begin{equation}
e^{\ri z \sin (\phi)} = \sum_{n=-\infty}^\infty  J_n(z) e^{\ri n\phi},
\end{equation}
{{</m>}}
the term $e^{2\ri \eta(r)}$ becomes
{{<m>}}
\begin{equation}
    \exp\left({\ri \frac{\lambda_1 \cos 2\theta_{\mm}}{k_1} \sin (k_1 r) }\right)  =  \sum_{n=-\infty}^{\infty} J_n \left( \frac{\lambda_1 \cos 2\theta_\mm}{k_1}\right) e^{\ri n k_1 r}.
\end{equation}
{{</m>}}
where $J_n(z)$ is the Bessel function of the first kind of order $n$. The Hamiltonian becomes a Rabi oscillation system with an infinite number of Rabi modes:
{{<m>}}
\begin{equation}
    \mathsf H^{(\mathrm{R})} =
    -\frac{\omega_{\mathrm{m}}}{2} \sigma_3
    -  \frac{1}{2} \sum_{n=-\infty}^\infty A_n \begin{pmatrix}
    0 &  e^{\ri n k_1  r} \\
     e^{ - \ri n k_1 r} & 0
    \end{pmatrix},
    \label{chap:matter-sec:jacobi-eqn:hamil-jacobi-expanded}
\end{equation}
{{</m>}}
where
{{<m>}}
\begin{align}
    A_n &= \tan 2\theta_{\mathrm m} n k_1 J_{n} \left( \frac{\lambda_1}{k_1}\cos 2\theta_{\mathrm m} \right)
\end{align}
{{</m>}}
and $n k_1$ are the amplitude and wavenumber of the $n$th Rabi mode.\footnote{A phase in the matter potential would contribute to the phases of the Rabi modes which do not play any role in the resonance for the reason discussed in Sec. \ref{chap:app-sec:rabi-oscillations}}
In obtaining Eqn. \eqref{chap:matter-sec:jacobi-eqn:hamil-jacobi-expanded}, I have used the following identity of the Bessel function
{{<m>}}
\begin{equation}
    J_{n-1}(z) + J_{n+1}(z) = \frac{2 n}{z} J_n(z).
    \label{eqn:bessel-function-sum-property}
\end{equation}
{{</m>}}


Eqn. \eqref{chap:matter-sec:jacobi-eqn:hamil-jacobi-expanded} implies an infinite number of resonance conditions
{{<m>}}
\begin{equation}
    \omega_\mm  = n k_1 \qquad (n=1, 2, \ldots)
    \label{chap:matter-sec:single-revisted-eqn:resonance-condition}
\end{equation}
{{</m>}}
However, the amplitude of the Rabi mode $A_n$ drops quickly as a function of $n$ because
{{<m>}}
\begin{equation}
    J_n(z) \xrightarrow{z\ll \sqrt{n+1}} \frac{ (z/2)^n }{n!} \qquad \text{if } n>0
    \label{chap:matter-sec:single-revisit-eqn:bessel-small-arg}
\end{equation}
{{</m>}}
when $\lambda_1/k_1 \ll 1$. For $\lambda_1/k_1\gtrsim 1$, $A_n$ also becomes small for sufficiently large $n$ because
{{<m>}}
\begin{equation}
    J_n(z) \xrightarrow{n\gg 1} \frac{1}{\sqrt{2\pi n}} \left( \frac{ e z }{ 2n } \right)^n.
\end{equation}
{{</m>}}
Any real physical system has a finite size $l$ and the Rabi modes with the oscillation wavelengths $2\pi/\Omega_n\sim 2\pi/A_n  \gtrsim l$ can be ignored even if they are on resonance.





In Sec. \ref{chap:matter-sec:single}, I have discussed the scenario where the $n=1$ Rabi mode is on or close to the resonance with $\lambda_1/\omega_\mm \ll 1$. Using Eqn. \eqref{chap:matter-sec:single-revisit-eqn:bessel-small-arg} and identity
{{<m>}}
\begin{equation}
    J_{-n}(z) =(-1)^n J_{n}(z)
\end{equation}
{{</m>}}
I obtain
{{<m>}}
\begin{equation}
    A_{\pm 1} \approx \frac{ \lambda_1 \sin (2\theta_\mm)}{2},
\end{equation}
{{</m>}}
which agrees with Eqn. \eqref{chap:matter-sec:single-eqn:rabi-amplitudes}. According to Eqn. \eqref{app:chap:matter-eq:relative-detuning-changed}, compared with the case where the first Rabi mode is present, the relative detuning of the Rabi resonance has a change of magnitude
{{<m>}}
\begin{equation}
\Delta \RD_{(n)} = \frac{1}{2} \frac{A_n}{A_1} \frac{1}{\RD_n}
\end{equation}
{{</m>}}
when another Rabi mode $n$ is present, where $\RD_n$ is the relative detuning when only the $n$th Rabi mode is considered. In Table \ref{table:relative-detunings-single-frequency-example}, I listed the values of $A_n/A_1$, $\RD_n$, and $\Delta \RD_{(n)}$ of a few off-resonance Rabi modes for the three numerical examples plotted in Fig. Neutrino Rabi Oscillations for Single Mode. One can see that all the off-resonance Rabi modes have very little impact on the resonance which explains why we could ignore the oscillating $\sigma_3$ terms in Eqn. \eqref{eq-hamiltonian-bg-matter-basis-single-frequency}.




|  | $k_1/\omega_{\mathrm m}=1$ | $k_1/\omega_\mm=1-2\times 10^{-5}$ | $k_1/\omega_\mm=1-10^{-4}$ |
|-----------------------|-------------------------------------------------|---------------------------------------------------------|------------------------------------------------|
| $n$                   | $A_n/A_1$                                       | $\RD_n$                                                 | $\Delta \RD_{(n)}$                             | $A_n/A_1$            | $\RD_n$            | $\Delta \RD_{(n)}$   | $A_n/A_1$            | $\RD_n$            | $\Delta \RD_{(n)}$   |
| -1                    | $1$                                             | $10^5$                                                  | $5\times 10^{-6}$                              | 1                    | $10^{5}$           | $5\times 10^{-6}$    | $1$                  | $10^{5}$           | $5\times 10^{-6}$    |
| 2                     | $4.8 \times 10^{-5}$                            | $1.1 \times 10^{9}$                                     | $2.2\times 10^{-14}$                           | $4.8 \times 10^{-5}$ | $1.1\times 10^9$   | $2.2\times 10^{-14}$ | $4.8 \times 10^{-5}$ | $1.1\times 10^9$   | $2.2\times 10^{-14}$ |
| $-2$                  | $4.8 \times 10^{-5}$                            | $3.2\times 10^{9}$                                      | $7.5\times 10^{-15}$                           | $4.8 \times 10^{-5}$ | $3.2\times 10^{9}$ | $7.5\times 10^{-15}$ | $4.8 \times 10^{-5}$ | $3.2\times 10^{9}$ | $7.6\times 10^{-15}$ |

Table relative-detunings-single-frequency-example shows the amplitudes and the relative detunings of a few Rabi modes and their impact on the Rabi resonance for the three numerical examples shown in Fig. Neutrino Rabi Oscillations for Single Mode.


